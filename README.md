<!--DOCTYPE html-->
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>7th Grade English - Unit 7 Lesson 2 (Workbook)</title>
    <style>
        body { 
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; 
            line-height: 1.6; 
            max-width: 850px; 
            margin: auto; 
            padding: 20px; 
            background-color: #e9ecef; 
            -webkit-user-select: none; 
            user-select: none; 
        }
        
        #main-container { 
            background: white; 
            padding: 30px; 
            border-radius: 15px; 
            box-shadow: 0 4px 15px rgba(0,0,0,0.1); 
            position: relative; 
        }
        
        #exam-content { display: none; }

        #lock-screen {
            display: none; 
            position: fixed; 
            top: 0; left: 0; 
            width: 100%; height: 100%;
            background: white; 
            color: #d9534f; 
            text-align: center; 
            padding-top: 50px; 
            z-index: 9999;
        }

        .header { 
            text-align: center; 
            border-bottom: 3px solid #007bff; 
            margin-bottom: 25px; 
            padding-bottom: 10px;
        }

        .question-box { 
            margin-bottom: 30px; 
            padding: 20px; 
            border: 1px solid #dee2e6; 
            border-radius: 10px; 
            background-color: #fff;
        }

        .word-bank {
            background-color: #f8f9fa;
            padding: 15px;
            border: 2px dashed #007bff;
            border-radius: 8px;
            margin-bottom: 15px;
            text-align: center;
            font-weight: bold;
        }
        
        .answer-line {
            border: none; 
            border-bottom: 2px solid #007bff; 
            width: 150px; 
            outline: none; 
            background: transparent;
            font-size: 16px;
            text-align: center;
            color: #495057;
        }

        .btn { padding: 12px 25px; cursor: pointer; border: none; border-radius: 5px; font-size: 16px; margin: 10px; font-weight: bold; transition: 0.3s; }
        .btn-start { background-color: #007bff; color: white; width: 280px; }
        .btn-start:hover { background-color: #0056b3; }
        .btn-submit { background-color: #28a745; color: white; width: 100%; margin-top: 20px; }
        .btn-submit:hover { background-color: #218838; }

        @media print { .no-print { display: none; } }
    </style>
</head>
<body>

<div id="lock-screen">
    <h1>⚠️ Activity Locked!</h1>
    <p style="font-size:20px; color:black;">School Activity Center</p>
    <p>You have already completed this activity or attempted to leave the page.</p>
    
    <div style="margin-top: 30px; border: 2px solid #ccc; display: inline-block; padding: 20px; border-radius: 10px;">
        <p style="color: blue;">Teacher Unlock Required:</p>
        <input type="password" id="teacher-password" placeholder="Enter PIN..." style="padding: 10px; font-size: 16px;">
        <button class="btn" onclick="unlockExam()" style="width: auto; background-color: #28a745; color:white;">Unlock</button>
        <p id="password-error" style="color: red; display: none;">Incorrect PIN!</p>
    </div>
</div>

<div id="main-container">
    <div id="start-area" style="text-align: center; padding: 50px;">
        <img src="https://img.icons8.com/color/96/000000/learning.png" alt="Learn"><br>
        <h2>Workbook Page 27</h2>
        <h3>Unit 7: WOW! Team Talk</h3>
        <p style="color: #6c757d;">Focus: Dialogue Completion and Reading Comprehension</p>
        <button class="btn btn-start" onclick="startExam()">Start Workbook Activity</button>
    </div>

    <div id="exam-content">
        <div class="header">
            <h1>Unit 7: Lesson 2 Interactive</h1>
            <div style="display: flex; justify-content: space-between; padding: 10px;">
                <div><strong>Student:</strong> <input type="text" id="studentName" placeholder="Enter Name..." class="answer-line" style="width: 200px;"></div>
                <div><strong>Grade:</strong> 6th Grade / Unit 7</div>
            </div>
        </div>

        <div class="question-box">
            <h3>1. Complete the sentences from the dialogue:</h3>
            <div class="word-bank">
                body | comedian | cool | costume | go | man | strings
            </div>
            <p>1. I like your clown <input type="text" id="v1" class="answer-line">, Arlo.</p>
            <p>2. They're difficult to <input type="text" id="v2" class="answer-line"> and they both have <input type="text" id="v3" class="answer-line">.</p>
            <p>3. Very <input type="text" id="v4" class="answer-line">, Faisal! You should be a <input type="text" id="v5" class="answer-line">.</p>
            <p>4. That's <input type="text" id="v6" class="answer-line">. Is he <input type="text" id="v7" class="answer-line">?</p>
            <p>5. What do you call a <input type="text" id="v8" class="answer-line"> with a big nose and no <input type="text" id="v9" class="answer-line">?</p>
            <p>6. Oh, it's time for the WOW! Talent Show. Let's <input type="text" id="v10" class="answer-line">!</p>
        </div>

        <div class="question-box">
            <h3>2. Answer the questions (Complete sentences):</h3>
            <p>1. Why is Arlo's costume a bit small?<br>
            <input type="text" id="q1" class="answer-line" style="width: 90%; text-align: left;"></p>
            
            <p>2. When did Arlo start to be a puppeteer?<br>
            <input type="text" id="q2" class="answer-line" style="width: 90%; text-align: left;"></p>
            
            <p>3. When did Faisal's uncle become a comedian?<br>
            <input type="text" id="q3" class="answer-line" style="width: 90%; text-align: left;"></p>
        </div>

        <div class="question-box">
            <h3>3. Read and complete the dialogues:</h3>
            <div class="word-bank">I've no idea | That's cool! | I get it!</div>
            <div style="font-style: italic; background: #f9f9f9; padding: 15px; border-radius: 5px;">
                <strong>Dialogue 1:</strong><br>
                <strong>A:</strong> I'm going to be in the talent show!<br>
                <strong>B:</strong> <input type="text" id="ex1" class="answer-line">! What's your talent?<br>
                <strong>A:</strong> Telling jokes! Why can't a bike stand up by itself?<br>
                <strong>B:</strong> <input type="text" id="ex2" class="answer-line">.<br>
                <strong>A:</strong> Because it's two-tyred! Do you understand?<br>
                <strong>B:</strong> Yes, <input type="text" id="ex3" class="answer-line">! That's funny!
            </div>
            <br>
            <div style="font-style: italic; background: #f9f9f9; padding: 15px; border-radius: 5px;">
                <strong>Dialogue 2:</strong><br>
                <strong>A:</strong> What time does the talent show start?<br>
                <strong>B:</strong> <input type="text" id="ex4" class="answer-line">. No one told me.<br>
                <strong>A:</strong> What are you going to do?<br>
                <strong>B:</strong> I'm going to make people laugh.<br>
                <strong>A:</strong> <input type="text" id="ex5" class="answer-line">! So are you a comedian?<br>
                <strong>B:</strong> No, I'm a puppeteer!<br>
                <strong>A:</strong> Oh, <input type="text" id="ex6" class="answer-line">! That's funny!
            </div>
        </div>
        
        <button class="btn btn-submit no-print" onclick="submitExam()">Finish and Show Results</button>
    </div>
</div>

<script>
    const TEACHER_SECRET = "0101"; 

    function startExam() {
        if (localStorage.getItem("wb_unit7_status") === "locked") {
            showLockScreen();
            return;
        }
        document.getElementById('start-area').style.display = 'none';
        document.getElementById('exam-content').style.display = 'block';
    }

    function submitExam() {
        let score = 0;
        const totalPoints = 19;
        const name = document.getElementById('studentName').value;
        if (!name) { alert("Please enter your name!"); return; }

        // Vocab Check (Based on Page 27, Exercise 1)
        const vocabAnswers = ["costume", "control", "strings", "funny", "comedian", "funny", "cool", "man", "body", "go"];
        for(let i=1; i<=10; i++) {
            let val = document.getElementById('v'+i).value.toLowerCase().trim();
            if(val === vocabAnswers[i-1]) score++;
        }

        // Questions Check (Keywords)
        if (document.getElementById('q1').value.toLowerCase().includes("long time")) score++;
        if (document.getElementById('q2').value.toLowerCase().includes("was seven")) score++;
        if (document.getElementById('q3').value.toLowerCase().includes("last year")) score++;

        // Expressions Check
        const expAnswers = ["cool", "no idea", "get it", "no idea", "cool", "get it"];
        for(let i=1; i<=6; i++) {
            if(document.getElementById('ex'+i).value.toLowerCase().includes(expAnswers[i-1])) score++;
        }

        alert(`Great job, ${name}!\nYour Score: ${score} / ${totalPoints}`);
        localStorage.setItem("wb_unit7_status", "locked");
        showLockScreen();
    }

    function showLockScreen() {
        document.getElementById('exam-content').style.display = 'none';
        document.getElementById('start-area').style.display = 'none';
        document.getElementById('lock-screen').style.display = 'block';
    }

    function unlockExam() {
        if (document.getElementById('teacher-password').value === TEACHER_SECRET) {
            localStorage.removeItem("wb_unit7_status");
            location.reload();
        } else {
            document.getElementById('password-error').style.display = 'block';
        }
    }

    document.addEventListener("visibilitychange", function() {
        if (document.hidden && document.getElementById('exam-content').style.display === 'block') {
            alert("Security Alert: Leaving the page will lock the activity!");
            localStorage.setItem("wb_unit7_status", "locked");
            showLockScreen();
        }
    });
</script>
</body>
</html>
