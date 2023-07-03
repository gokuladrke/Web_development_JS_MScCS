# Advanced Java

- [Advanced Java](#advanced-java)
  - [Announcements](#announcements)
  - [Schedule](#schedule)
  - [Session - 1 Contents](#july-3rd-2023)

## Announcements

<script>
  var countDownDate = new Date("Jul 3, 2023 09:30:00").getTime();
  var myfunc = setInterval(function() {
    var now = new Date().getTime();
    var timeleft = countDownDate - now;
        
    // Calculating the days, hours, minutes and seconds left
    var days = Math.floor(timeleft / (1000 * 60 * 60 * 24));
    var hours = Math.floor((timeleft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    var minutes = Math.floor((timeleft % (1000 * 60 * 60)) / (1000 * 60));
    var seconds = Math.floor((timeleft % (1000 * 60)) / 1000);

    var lastDate = new Date("Jul 7, 2023 12:45:00");

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

- Please make use of the [comment](#write-your-comments-below) section in the end of the page for any doubts/clarifications needed related to the training.
- The training page will have everything related to the training from schedules to quizzes.

## Schedule

| Agenda                                      | Date       | Time              | Training Venue | Tools Used                   |
| ------------------------------------------- | ---------- | ----------------- | -------------- | ---------------------------- |
| Introducing Classes                         | 03.07.2023 | 9.30am to 12.30am | VM Hall        | VS Code, Google Form         |
| A Closer look at Methods and Classes        | 04.07.2023 | 9.30am to 12.30am | VM Hall        | Slides, Google Form, VS Code |
| Inheritance                                 | 06.07.2023 | 9.30am to 12.30am | VM Hall        | Slides, Google Form, VS Code |
| Packages, Interfaces and Exception Handling | 07.07.2023 | 9.30am to 12.30am | VM Hall        | Slides, Google Form, VS Code |

## July 3rd 2023

| Time                | Topic                                                   | Details | Link                                                                                                         |
| ------------------- | ------------------------------------------------------- | ------- | ------------------------------------------------------------------------------------------------------------ |
| 9.30am to 11.00am   | Faculty Introduction & Setting up the Stage             | 5 mins  | [Faculty Introduction & Setting up the Stage](faculty.md)                                                    |
|                     | How to use the Training page?                           | 5 mins  |                                                                                                              |
|                     | Github Registration and Joining slack for communication | 5 mins  | [Joining slack](https://join.slack.com/t/rvscas-workspace/shared_invite/zt-1mss74s1x-4hZOxPeIpd1Tp2mQXxipOg) |
|                     | Class Fundamentals                                      | 20 mins |                                                                                                              |
|                     | Declaring Objects                                       | 20 mins |                                                                                                              |
|                     | Assigning Object Reference Variables                    | 20 mins |                                                                                                              |
|                     | Q & A                                                   | 15 mins | [Padlet](https://padlet.com/sathishdatascientist/javaPadlet)                                                 |
| 11.00 am to 11.15am | Tea Break & Refreshments                                |         |                                                                                                              |
| 11.15am to 12.30pm  | Declaring Methods                                       | 15 mins |                                                                                                              |
|                     | Returning a Value                                       | 15 mins |                                                                                                              |
|                     | Adding a Method that takes parameters                   | 15 mins |                                                                                                              |
|                     | Q & A                                                   | 15 mins | [Padlet](https://padlet.com/sathishdatascientist/javaPadlet)                                                 |
|                     | Test your understanding - Quiz                          | 15 mins | [Quiz](https://forms.gle/zKYJWGqJTphbKR7W7)                                                                  |

## Homeworks

| Topic                                       | Release Date | Deadline | Link |
| ------------------------------------------- | ------------ | -------- | ---- |
| Introducing Classes                         |              |          |      |
| A Closer look at Methods and Classes        |              |          |      |
| Inheritance                                 |              |          |      |
| Packages, Interfaces and Exception Handling |              |          |      |

## Write your comments below

<script 
        async
        src="https://utteranc.es/client.js"
        repo="casrvs/casrvs.github.io"
        issue-term="title"
        theme="github-light"
        crossorigin="anonymous"
></script>
