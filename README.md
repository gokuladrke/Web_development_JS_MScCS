# Web Development with JavaScript

- [Web Developmentwith JS](#wdjs)
  - [Announcements](#announcements)
  - [Syllabus](./syllabus/WDJS.pdf)
  - [Schedule](#schedule)
  - [Session - 1 Contents](#january-1)
  - [Schedule for Week 5](#week-5-schedule)

## Announcements

<script>
  var countDownDate = new Date("Feb 20, 2023 09:30:00").getTime();
  var myfunc = setInterval(function() {
    var now = new Date().getTime();
    var timeleft = countDownDate - now;
        
    // Calculating the days, hours, minutes and seconds left
    var days = Math.floor(timeleft / (1000 * 60 * 60 * 24));
    var hours = Math.floor((timeleft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    var minutes = Math.floor((timeleft % (1000 * 60 * 60)) / (1000 * 60));
    var seconds = Math.floor((timeleft % (1000 * 60)) / 1000);

    var lastDate = new Date("Feb 24, 2023 12:45:00");

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

- Syllabus for Web Development with JavaScript given.
- Have to take up  Knowledge check after each concepts.
- Coding Activity and Coding Assignments to be submitted within stipulated time.
- Please make use of the [comment](#write-your-comments-below) section in the end of the page for any doubts/clarifications needed related to the class.



## Schedule

|     Setting up your System    | Introduction   And Instructions     | Introduction   And Instructions                                                   |
|:-----------------------------:|-------------------------------------|-----------------------------------------------------------------------------------|
|                               | Introduction   To The Command Line  | Command   Line And File System                                                    |
|                               | Command   Line Shells: Zsh And Bash | Zsh   And Git Bash                                                                |
|                               | Setting   Up Command Line Shells    | Setting   Up Command Line Shells                                                  |
|                               | Using   The Terminal                | Mac   Terminal,Windows Terminal,Linux Terminal                                    |
|                               | Discussion   0.1                    | Customize   Your Terminal                                                         |
|                               | Code   Style Introduction           | Code   Style Introduction And Style Guide                                         |
|                               | JavaScript   Resources              | JavaScript   Resources                                                            |
|                               | Discussion   0.2                    | Examine   JavaScript Resources                                                    |
|                               | Introducing   VS Code               | Introducing   VS Code,Command Line Shell And VS Code Set Up Troubleshooting Guide |
|                               | Discussion   0.3                    | Setting   Up VS Code                                                              |
|                               | Getting   Started With GitHub       | Introduction   To GitHub And GitHub Exercise,Crash Course On Git                  |
|                               | Discussion_0.4                      | How   to Create Your Own Web Page In GitHub                                       |
|                               | Additional   Resources              | Additional   Resources                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |

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
