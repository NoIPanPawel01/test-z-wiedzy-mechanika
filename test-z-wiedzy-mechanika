<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quiz</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f9;
            color: #333;
            margin: 0;
            padding: 20px;
        }
        .quiz-container {
            max-width: 700px;
            margin: 50px auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }
        .quiz-header {
            text-align: center;
            margin-bottom: 20px;
        }
        .progress-bar {
            height: 10px;
            background: #e0e0e0;
            border-radius: 5px;
            overflow: hidden;
            margin-bottom: 20px;
        }
        .progress-bar-fill {
            width: 0;
            height: 100%;
            background: #4CAF50;
            transition: width 0.3s ease-in-out;
        }
        .question {
            margin-bottom: 20px;
        }
        .answers label {
            display: block;
            margin: 5px 0;
            padding: 10px;
            background: #f9f9f9;
            border: 1px solid #ddd;
            border-radius: 5px;
            cursor: pointer;
        }
        .answers input {
            margin-right: 10px;
        }
        button {
            display: block;
            margin: 20px auto;
            padding: 10px 20px;
            font-size: 16px;
            color: white;
            background: #4CAF50;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        button:hover {
            background: #45a049;
        }
        .result-overlay {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.7);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }
        .result-box {
            background: white;
            padding: 30px;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
        }
        .result-box h2 {
            margin: 0 0 20px;
        }
    </style>
</head>
<body>
    <div class="quiz-container">
        <div class="quiz-header">
            <h1>Test z wiedzy mechanika 😏</h1>
            <div class="progress-bar">
                <div class="progress-bar-fill" id="progress-bar-fill"></div>
            </div>
        </div>
        <form id="quiz-form">
            <div class="question">
                </div>
                <p>1. Jaką jednostką mierzymy siłę?</p>
                <div class="answers">
                    <label><input type="radio" name="q1" value="a"> Newton</label>
                    <label><input type="radio" name="q1" value="b"> Kilogram</label>
                    <label><input type="radio" name="q1" value="c"> Dżul</label>
                    <label><input type="radio" name="q1" value="d"> Watt</label>
                </div>
            </div>
            <div class="question">
                <p>2. Co to jest prędkość?</p>
                <div class="answers">
                    <label><input type="radio" name="q2" value="a"> Szybkość poruszania się ciała</label>
                    <label><input type="radio" name="q2" value="b"> Siła, która działa na ciało</label>
                    <label><input type="radio" name="q2" value="c"> Siła, która przyśpiesza ciało</label>
                    <label><input type="radio" name="q2" value="d"> Siła, która zatrzymuje ciało</label>
                </div>
            </div>
            <div class="question">
                <p>3. Co to jest tarcie?</p>
                <div class="answers">
                    <label><input type="radio" name="q3" value="a"> Siła, która pomaga ciału się poruszać</label>
                    <label><input type="radio" name="q3" value="b"> Siła, która utrudnia ruch ciała</label>
                    <label><input type="radio" name="q3" value="c"> Siła, która przyśpiesza ciało</label>
                    <label><input type="radio" name="q3" value="d"> Siła, która zatrzymuje ciało</label>
                </div>
            </div>
            <div class="question">
                <p>4. Jak nazywamy energię związaną z ruchem ciała?</p>
                <div class="answers">
                    <label><input type="radio" name="q4" value="a"> Energia Kinetyczna</label>
                    <label><input type="radio" name="q4" value="b"> Energia Potencjalna</label>
                    <label><input type="radio" name="q4" value="c"> Energia sprężystości</label>
                    <label><input type="radio" name="q4" value="d"> Energia elektryczna</label>
                </div>
            </div>
            <div class="question">
                <p>5. Co to jest praca mechaniczna?</p>
                <div class="answers">
                    <label><input type="radio" name="q5" value="a"> Zmiana prędkości ciała</label>
                    <label><input type="radio" name="q5" value="b"> Siła, która powoduje ruch ciała</label>
                    <label><input type="radio" name="q5" value="c"> Przemieszczanie ciała pod wpływem siły</label>
                    <label><input type="radio" name="q5" value="d"> Energia ciała ruchu</label>
                </div>
            </div>
            <div class="question">
                <p>6. 15 Mil ile to Km?</p>
                <div class="answers">
                    <label><input type="radio" name="q6" value="a"> 15 Km</label>
                    <label><input type="radio" name="q6" value="b"> 24 Km</label>
                    <label><input type="radio" name="q6" value="c"> 28 Km</label>
                    <label><input type="radio" name="q6" value="d"> 12 Km</label>
                </div>
            </div>
            <div class="question">
                <p>7. Ile 1 HP to KM?</p>
                <div class="answers">
                    <label><input type="radio" name="q7" value="a"> 1.08KM</label>
                    <label><input type="radio" name="q7" value="b"> 1.01KM</label>
                    <label><input type="radio" name="q7" value="c"> 1.11KM</label>
                    <label><input type="radio" name="q7" value="d"> 1.00KM</label>
                </div>
            </div>
            <div class="question">
                <p>8. Co mierzymy w dżulach?</p>
                <div class="answers">
                    <label><input type="radio" name="q8" value="a"> Siłę</label>
                    <label><input type="radio" name="q8" value="b"> Energię</label>
                    <label><input type="radio" name="q8" value="c"> Prędkość</label>
                    <label><input type="radio" name="q8" value="d"> Czas</label>
                </div>
            </div>
            <div class="question">
                <p>9. Jaki silnik ma Mazda RX-7?</p>
                <div class="answers">
                    <label><input type="radio" name="q9" value="a"> Wankla</label>
                    <label><input type="radio" name="q9" value="b"> Hemi</label>
                    <label><input type="radio" name="q9" value="c"> Bokser</label>
                </div>
            </div>
            <div class="question">
                <p>10. Co to jest przyśpieszenie?</p>
                <div class="answers">
                    <label><input type="radio" name="q10" value="a"> Zmiana w jednostce prędkości czasu</label>
                    <label><input type="radio" name="q10" value="b"> Prędkość ciała</label>
                    <label><input type="radio" name="q10" value="c"> Siła, która działa na ciało</label>
                    <label><input type="radio" name="q10" value="d"> Energia ciała</label>
                </div>
            </div>
            <p>11. Na ile dokręcamy koła w samochodzie nie ciężarowym?</p>
                <div class="answers">
                    <label><input type="radio" name="q11" value="a"> 100 Nm</label>
                    <label><input type="radio" name="q11" value="b"> 140 Nm</label>
                    <label><input type="radio" name="q11" value="c"> 180 Nm</label> 
                    <label><input type="radio" name="q11" value="d"> 200 Nm</label>
                </div>
            </div>
            <p>12. Alternator w samochodzie służy do?</p>
                <div class="answers">
                    <label><input type="radio" name="q12" value="a"> Utrzymanie stałej prędkości</label>
                    <label><input type="radio" name="q12" value="b"> wytwarzanie prądu</label>
                </div>
            </div>
            <p>13. Klucz dynamometryczny służy do?</p>
                <div class="answers">
                    <label><input type="radio" name="q13" value="a"> Dokręcanie śrub odpowiednim momentem obrotowym</label>
                    <label><input type="radio" name="q13" value="b"> Ustawianie reflektorów na odpowiedniej wysokości</label>
                </div>
            </div>
            <p>14. Jakie zadanie ma wałek rozrządu w silniku?</p>
                <div class="answers">
                    <label><input type="radio" name="q14" value="a"> Przekazuje moment obrotowy między skrzynią biegów a kołami</label>
                    <label><input type="radio" name="q14" value="b"> Steruje otwarciem zaworów ssących i wydechowych</label>
                </div>
            </div>
            <p>15. Cztery fazy pracy tłoka w silniku spalinowym  ssanie - sprężanie - praca - ?</p>
                <div class="answers">
                    <label><input type="radio" name="q15" value="a"> Suw</label>
                    <label><input type="radio" name="q15" value="b"> Zapłon</label>
                    <label><input type="radio" name="q15" value="c"> Powrót</label>
                    <label><input type="radio" name="q15" value="d"> Wydech</label>
                </div>
            </div>
            <button type="button" onclick="submitQuiz()">Zakończ test</button>
        </form>
    </div>

    <!-- Wynik -->
    <div class="result-overlay" id="result-overlay">
        <div class="result-box">
            <h2 id="result-text"></h2>
            <button onclick="closeResult()">Zamknij</button>
        </div>
    </div>

    <script>
        const correctAnswers = {
            q1: 'a',
            q2: 'a',
            q3: 'b',
            q4: 'a',
            q5: 'c',
            q6: 'b',
            q7: 'b',
            q8: 'a',
            q9: 'a',
            q10: 'a',
            q11: 'b',
            q12: 'b',
            q13: 'a',
            q14: 'b',
            q15: 'd',
        };

        function submitQuiz() {
            const form = document.getElementById('quiz-form');
            const formData = new FormData(form);
            let score = 0;
            const totalQuestions = Object.keys(correctAnswers).length;

            // Sprawdzanie odpowiedzi
            for (const [question, answer] of formData.entries()) {
                if (correctAnswers[question] === answer) {
                    score++;
                }
            }

            // Wyświetlenie wyniku
            const resultOverlay = document.getElementById('result-overlay');
            const resultText = document.getElementById('result-text');
            resultText.textContent = `Twój wynik: ${score}/${totalQuestions}`;
            resultOverlay.style.display = 'flex';

            // Aktualizacja paska postępu
            const progressBar = document.getElementById('progress-bar-fill');
            progressBar.style.width = `${(score / totalQuestions) * 100}%`;
        }

        function closeResult() {
            const resultOverlay = document.getElementById('result-overlay');
            resultOverlay.style.display = 'none';
        }
    </script>
</body>
</html>
