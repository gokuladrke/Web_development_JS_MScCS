# Data Structures and Algorithms Using Java

- [DSA Using Java](#dsa-using-java)
  - [Announcements](#announcements)
  - [Schedule](#schedule)
  - [Session - 1 Contents](#january-1)

## Announcements

<script>
  var countDownDate = new Date("Jan 09, 2023 09:30:00").getTime();
  var myfunc = setInterval(function() {
    var now = new Date().getTime();
    var timeleft = countDownDate - now;
        
    // Calculating the days, hours, minutes and seconds left
    var days = Math.floor(timeleft / (1000 * 60 * 60 * 24));
    var hours = Math.floor((timeleft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    var minutes = Math.floor((timeleft % (1000 * 60 * 60)) / (1000 * 60));
    var seconds = Math.floor((timeleft % (1000 * 60)) / 1000);

    var lastDate = new Date("Jan 13, 2023 12:45:00");

    if(now<countDownDate){
      document.getElementById("time").innerHTML = 'The Training starts in ' + days + ' days ' + hours + ' hours ' + minutes + ' minutes ' + seconds + ' seconds <br /> <br />';
    } else if(now>=countDownDate && now<=lastDate){
      document.getElementById("time").innerHTML = 'The Training is LIVE! <br /> <br />';
    } else if(now>lastDate){
      document.getElementById("time").innerHTML = 'The Training is COMPLETED! <br /> <br />';
    }

  },1000);
</script>

<div>
  <ul>
    <li id='time'></li>
  </ul>
</div>

- January 11 & 12 Schedules added!
- Quiz in January 9th Schedule is enabled!
- Homework for January 12 is added. Deadline for the homework submission is 13th Jan 11:59 PM.
- Please make use of the [comment](#write-your-comments-below) section in the end of the page for any doubts/clarifications needed related to the training.
- The training page will have everything related to the training from schedules to quizzes.

## Schedule

| Agenda                                                    | Date       | Time              | Training Venue | Tools Used                   |
| --------------------------------------------------------- | ---------- | ----------------- | -------------- | ---------------------------- |
| Introduction and Abstract Data Types, Asymptotic Analysis | 09.01.2023 | 9.30am to 12.30am | VM Hall        | Github, Slides, Google Form  |
| Arrays and Recursion                                      | 10.01.2023 | 9.30am to 12.30am | VM Hall        | Slides, Google Form, VS Code |
| Linked Lists - Introduction                               | 11.01.2023 | 9.30am to 12.30am | VM Hall        | Slides, Google Form, VS Code |
| Singly Linked Lists                                       | 12.01.2023 | 9.30am to 12.30am | VM Hall        | Slides, Google Form, VS Code |
| Doubly Linked Lists and Circularly Linked Lists           | 13.01.2023 | 9.30am to 12.30am | VM Hall        | Slides, Google Form, VS Code |

## January 9

| Time                | Topic                                                    | Details | Link                                                                                                                                                                                     |
| ------------------- | -------------------------------------------------------- | ------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 9.30am to 11.00am   | Faculty Introduction & Setting up the Stage              | 5 mins  | [Faculty Introduction & Setting up the Stage](faculty.md)                                                                                                                                |
|                     | How to use the Training page?                            | 5 mins  |                                                                                                                                                                                          |
|                     | Github Registration and Joining slack for communication  | 5 mins  | [Joining slack](https://join.slack.com/t/rvscas-workspace/shared_invite/zt-1mss74s1x-4hZOxPeIpd1Tp2mQXxipOg)                                                                             |
|                     | Variables and Data Types - Primitive and User-Defined    | 15 mins | [Slides](./slides/variables-and-data-types.md), [Lecture Notes](./lectureNotes/variables-datatypes.md), [Knowledge Check](https://forms.gle/cK253ecaAwFhSpfc8)                           |
|                     | Introduction - Data Structures, Abstract Data Types      | 15 mins | [Slides](./slides/data-structures-and-adt.md),[Lecture Notes](./lectureNotes/data-structures-abstract-data-types.md), [Knowledge Check](https://forms.gle/4SNofPENpZCdAAdu8)             |
|                     | What is an Algorithm? Asymptotic Notations and its Types | 30 mins | [Slides](./slides/algorithms-and-asymptotic-notations.md),[Lecture Notes](./lectureNotes/algorithms-and-asymptotic-notations.md), [Knowledge Check](https://forms.gle/fokYZ1hgrehWSsABA) |
|                     | Q & A                                                    | 15 mins | [Padlet](https://padlet.com/sathishdatascientist/oqf09oefydef834j)                                                                                                                       |
| 11.00 am to 11.15am | Tea Break & Refreshments                                 |         |                                                                                                                                                                                          |
| 11.15am to 12.30pm  | Representing an algorithm as a Pseudocode                | 15 mins | [Slides](./slides/pseudocode.md)                                                                                                                                                         |
|                     | Pseudocode Example - Fibonacci Series                    | 30 mins |                                                                                                                                                                                          |
|                     | Q & A                                                    | 15 mins | [Padlet](https://padlet.com/sathishdatascientist/oqf09oefydef834j)                                                                                                                       |
|                     | Test your understanding - Quiz                           | 15 mins | [Quiz](https://forms.gle/VQDWiFv6GxRRofS69)                                                                                                                                              |

## January 10

| Time                | Topic                          | Details | Link                                                               |
| ------------------- | ------------------------------ | ------- | ------------------------------------------------------------------ |
| 9.30am to 11.00am   | Revisiting Abstract Data Types | 30 mins |                                                                    |
|                     | Q&A                            | 15 mins |                                                                    |
|                     | Algorithms and Pseudocodes     | 45 mins |                                                                    |
|                     | Q & A                          | 15 mins | [Padlet](https://padlet.com/sathishdatascientist/oqf09oefydef834j) |
| 11.00 am to 11.15am | Tea Break & Refreshments       |         |                                                                    |
| 11.15am to 12.30pm  | Arrays                         | 10 mins | [Slides](./slides/arrays.md)                                       |
|                     | Recursion                      | 20 mins | [Slides](./slides/recursion.md)                                    |
|                     | Q & A                          | 5 mins  | [Padlet](https://padlet.com/sathishdatascientist/oqf09oefydef834j) |
|                     | Test your understanding - Quiz | 10 mins | [Quiz]()                                                           |

## January 11

| Time               | Topic                            | Details | Link                                                               |
| ------------------ | -------------------------------- | ------- | ------------------------------------------------------------------ |
| 9.30am to 11.00am  | Revisiting Abstract Data Types   | 30 mins |                                                                    |
|                    | Q & A                            | 15 mins | [Padlet](https://padlet.com/sathishdatascientist/oqf09oefydef834j) |
| 11.15am to 11.30am | Tea Break & Refreshments         | 15 mins |                                                                    |
| 11.30am to 1.15pm  | Problem Solving                  | 80 mins | [Notes](./lectureNotes/pseudocode.md)                              |
|                    | Assignment Instructions and Demo | 15 mins | [Slides](./lectureNotes/assignment-instructions.md)                |

## January 12

| Time               | Topic                           | Details | Link                                                               |
| ------------------ | ------------------------------- | ------- | ------------------------------------------------------------------ |
| 9.30am to 10.30am  | Assignment Hands-On with GitHub | 30 mins | [Instructions](./lectureNotes/assignment-instructions.md)          |
| 10.30am to 11.15am | Recursion                       | 45 mins | [Padlet](https://padlet.com/sathishdatascientist/oqf09oefydef834j) |
| 11.15am to 11.30am | Tea Break & Refreshments        | 15 mins |                                                                    |
| 11.30am to 12.45pm | Linked Lists - Introduction     | 60 mins | [Notes](./slides/pseudocode.md)                                    |
|                    | Q&A                             | 15 mins | [Padlet](https://padlet.com/sathishdatascientist/oqf09oefydef834j) |

## Homeworks

| Topic                | Release Date | Deadline             | Link                                            |
| -------------------- | ------------ | -------------------- | ----------------------------------------------- |
| Asymptotic Notations | 12-Jan-2023  | 13-Jan-2023 11:59 PM | [Homework](https://forms.gle/jN8jxmpeSpwzM6BQ6) |
| Arrays               |              |                      |                                                 |
| Recursion            |              |                      |                                                 |
| Linked Lists         |              |                      |                                                 |

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
