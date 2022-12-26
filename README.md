# Data Structures and Algorithms Using Java

- [DSA Using Java](#dsa-using-java)
  - [Announcements](#announcements)
  - [Schedule](#schedule)

## Announcements

<script>
  var countDownDate = new Date("Jan 02, 2023 09:30:00").getTime();
  var myfunc = setInterval(function() {
    var now = new Date().getTime();
    var timeleft = countDownDate - now;
        
    // Calculating the days, hours, minutes and seconds left
    var days = Math.floor(timeleft / (1000 * 60 * 60 * 24));
    var hours = Math.floor((timeleft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    var minutes = Math.floor((timeleft % (1000 * 60 * 60)) / (1000 * 60));
    var seconds = Math.floor((timeleft % (1000 * 60)) / 1000);

    document.getElementById("time").innerHTML = 'The Training starts in ' + days + ' days ' + hours + ' hours ' + minutes + ' minutes ' + seconds + ' seconds <br /> <br />';
  },1000);
</script>
<ul>
  <li id='time'></li>
  <li markdown = "1">Please make use of the [comment](#write-your-comments-below) section in the end of the page for any doubts/clarifications needed related to the training.
- The training page will have everything related to the training from schedules to quizzes.

## Schedule

| Agenda                                                    | Date       | Time              | Training Venue | Tools Used                   |
| --------------------------------------------------------- | ---------- | ----------------- | -------------- | ---------------------------- |
| Introduction and Abstract Data Types, Asymptotic Analysis | 02.01.2023 | 9.30am to 12.30am | VM Hall        | Github, Slides, Google Form  |
| Arrays and Recursion                                      | 03.01.2023 | 9.30am to 12.30am | VM Hall        | Slides, Google Form, VS Code |
| Linked Lists - Introduction                               | 04.01.2023 | 9.30am to 12.30am | VM Hall        | Slides, Google Form, VS Code |
| Singly Linked Lists                                       | 05.01.2023 | 9.30am to 12.30am | VM Hall        | Slides, Google Form, VS Code |
| Doubly Linked Lists and Circularly Linked Lists           | 06.01.2023 | 9.30am to 12.30am | VM Hall        | Slides, Google Form, VS Code |

<!-- ## Pattern of the Test

| Section           | Questions    | Time    |
| ----------------- | ------------ | ------- |
| Programming Logic | 10 Questions | 15 Mins |
| Hands-On Coding   | 1 Question   | 15 Mins |
| Hands-On Coding   | 1 Questions  | 30 Mins | -->

## Write your comments below

<script 
        async
        src="https://utteranc.es/client.js"
        repo="casrvs/casrvs.github.io"
        issue-term="title"
        theme="github-light"
        crossorigin="anonymous"
></script>
