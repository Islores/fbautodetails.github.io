<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Flores and Damon's Car Quiz</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #111;
      color: #fff;
      text-align: center;
      padding: 20px;
    }
    h1 {
      color: #ffcc00;
    }
    .quiz-container {
      max-width: 600px;
      margin: auto;
      background: #222;
      padding: 20px;
      border-radius: 10px;
    }
    img {
      width: 100%;
      border-radius: 10px;
      margin: 10px 0;
    }
    button {
      margin: 10px;
      padding: 10px 20px;
      font-size: 16px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      background: #ffcc00;
      color: #000;
    }
    button:hover {
      background: #ffaa00;
    }
  </style>
</head>
<body>
  <h1>🚗 Flores and Damon's Car Quiz 🚗</h1>
  <div class="quiz-container">
    <div id="question-container"></div>
    <div id="answer-buttons"></div>
    <button id="next-btn" style="display:none;">Next</button>
    <h2 id="score-container" style="display:none;"></h2>
  </div>

  <script>
    const questions = [
      {
        question: "What is the 0-60 time of the Corvette C7 Stingray?",
        image: "https://upload.wikimedia.org/wikipedia/commons/7/7d/2014_Chevrolet_Corvette_stingray_Z51_coupe_--_03-09-2013.jpg",
        answers: [
          { text: "3.8 seconds", correct: true },
          { text: "5.0 seconds", correct: false },
          { text: "4.5 seconds", correct: false },
          { text: "2.9 seconds", correct: false }
        ]
      },
      {
        question: "Which company makes the AMG performance line?",
        image: "https://upload.wikimedia.org/wikipedia/commons/4/4e/2018_Mercedes-AMG_GT_C_Premium_Auto_4.0_Front.jpg",
        answers: [
          { text: "BMW", correct: false },
          { text: "Mercedes-Benz", correct: true },
          { text: "Audi", correct: false },
          { text: "Porsche", correct: false }
        ]
      },
      {
        question: "What is the 0-60 time of a Tesla Model S Plaid?",
        image: "https://upload.wikimedia.org/wikipedia/commons/8/87/Tesla_Model_S_Plaid_IMG_4342.jpg",
        answers: [
          { text: "1.9 seconds", correct: true },
          { text: "3.2 seconds", correct: false },
          { text: "2.5 seconds", correct: false },
          { text: "4.0 seconds", correct: false }
        ]
      },
      {
        question: "Ferrari’s logo features what animal?",
        image: "https://upload.wikimedia.org/wikipedia/en/thumb/3/3d/Ferrari-Logo.svg/1200px-Ferrari-Logo.svg.png",
        answers: [
          { text: "Horse", correct: true },
          { text: "Bull", correct: false },
          { text: "Lion", correct: false },
          { text: "Tiger", correct: false }
        ]
      },
      {
        question: "Which car is nicknamed 'Godzilla'?",
        image: "https://upload.wikimedia.org/wikipedia/commons/f/f6/Nissan_GT-R_in_Tokyo.JPG",
        answers: [
          { text: "Toyota Supra", correct: false },
          { text: "Nissan GT-R", correct: true },
          { text: "Mazda RX-7", correct: false },
          { text: "Acura NSX", correct: false }
        ]
      },
      {
        question: "What’s the 0-60 time of the Dodge Demon 170?",
        image: "https://upload.wikimedia.org/wikipedia/commons/5/5b/Dodge_Challenger_SRT_Demon.jpg",
        answers: [
          { text: "1.6 seconds", correct: true },
          { text: "2.8 seconds", correct: false },
          { text: "3.5 seconds", correct: false },
          { text: "4.1 seconds", correct: false }
        ]
      },
      {
        question: "Which Italian brand is famous for the Aventador?",
        image: "https://upload.
