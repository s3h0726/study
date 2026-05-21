<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>스터디 플래너</title>

  <style>
    body{
      margin:0;
      font-family: "Pretendard", sans-serif;
      background:#0f172a;
      color:white;
      padding:30px;
    }

    h1{
      text-align:center;
      margin-bottom:30px;
    }

    .container{
      display:grid;
      grid-template-columns: 1fr 1fr;
      gap:20px;
    }

    .card{
      background:#1e293b;
      padding:20px;
      border-radius:20px;
      box-shadow:0 4px 15px rgba(0,0,0,0.3);
    }

    input, button, select{
      padding:10px;
      border:none;
      border-radius:10px;
      margin-top:10px;
      font-size:15px;
    }

    input, select{
      width:100%;
      background:#334155;
      color:white;
    }

    button{
      background:#3b82f6;
      color:white;
      cursor:pointer;
      width:100%;
      transition:0.2s;
    }

    button:hover{
      background:#2563eb;
    }

    ul{
      list-style:none;
      padding:0;
    }

    li{
      background:#334155;
      padding:10px;
      border-radius:10px;
      margin-top:10px;
    }

    .timer{
      font-size:40px;
      text-align:center;
      margin:20px 0;
      font-weight:bold;
    }

    .subject-item{
      display:flex;
      justify-content:space-between;
      align-items:center;
    }

    .calendar-task{
      margin-top:10px;
    }

    @media(max-width:800px){
      .container{
        grid-template-columns:1fr;
      }
    }
  </style>
</head>
<body>

  <h1>📚 Study Planner</h1>

  <div class="container">

    <!-- 과목 추가 -->
    <div class="card">
      <h2>과목 관리</h2>

      <input type="text" id="subjectInput" placeholder="과목 이름 입력">

      <button onclick="addSubject()">과목 추가</button>

      <ul id="subjectList"></ul>
    </div>

    <!-- 공부 시간 측정 -->
    <div class="card">
      <h2>공부 시간 측정</h2>

      <select id="subjectSelect"></select>

      <div class="timer" id="timer">00:00:00</div>

      <button onclick="startTimer()">시작</button>
      <button onclick="stopTimer()">정지</button>

      <h3>누적 공부 시간</h3>
      <ul id="timeList"></ul>
    </div>

    <!-- 캘린더 -->
    <div class="card">
      <h2>📅 공부 일정 추가</h2>

      <input type="date" id="dateInput">

      <input type="text" id="taskInput" placeholder="공부할 내용 입력">

      <button onclick="addTask()">일정 추가</button>

      <ul id="taskList"></ul>
    </div>

  </div>

  <script>
    let subjects = [];
    let studyTimes = {};

    function addSubject(){
      const input = document.getElementById("subjectInput");
      const subject = input.value.trim();

      if(subject === "") return;

      subjects.push(subject);
      studyTimes[subject] = 0;

      updateSubjects();

      input.value = "";
    }

    function updateSubjects(){
      const subjectList = document.getElementById("subjectList");
      const subjectSelect = document.getElementById("subjectSelect");
      const timeList = document.getElementById("timeList");

      subjectList.innerHTML = "";
      subjectSelect.innerHTML = "";
      timeList.innerHTML = "";

      subjects.forEach(subject => {

        // 과목 목록
        const li = document.createElement("li");
        li.className = "subject-item";
        li.innerHTML = `<span>${subject}</span>`;
        subjectList.appendChild(li);

        // 셀렉트 옵션
        const option = document.createElement("option");
        option.value = subject;
        option.textContent = subject;
        subjectSelect.appendChild(option);

        // 시간 표시
        const timeLi = document.createElement("li");
        timeLi.textContent =
          `${subject} : ${formatTime(studyTimes[subject])}`;
        timeList.appendChild(timeLi);
      });
    }

    let timer;
    let seconds = 0;
    let currentSubject = "";

    function startTimer(){

      currentSubject =
        document.getElementById("subjectSelect").value;

      if(currentSubject === "") return;

      clearInterval(timer);

      timer = setInterval(() => {
        seconds++;
        studyTimes[currentSubject]++;

        document.getElementById("timer").textContent =
          formatTime(seconds);

        updateSubjects();
      }, 1000);
    }

    function stopTimer(){
      clearInterval(timer);
      seconds = 0;

      document.getElementById("timer").textContent =
        "00:00:00";
    }

    function formatTime(sec){

      let h = Math.floor(sec / 3600);
      let m = Math.floor((sec % 3600) / 60);
      let s = sec % 60;

      return (
        String(h).padStart(2,"0") + ":" +
        String(m).padStart(2,"0") + ":" +
        String(s).padStart(2,"0")
      );
    }

    // 일정 추가
    function addTask(){

      const date =
        document.getElementById("dateInput").value;

      const task =
        document.getElementById("taskInput").value;

      if(date === "" || task === "") return;

      const li = document.createElement("li");
      li.className = "calendar-task";

      li.innerHTML =
        `<strong>${date}</strong><br>${task}`;

      document.getElementById("taskList")
        .appendChild(li);

      document.getElementById("taskInput").value = "";
    }

  </script>

</body>
</html>
