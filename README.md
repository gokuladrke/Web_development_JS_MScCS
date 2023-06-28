# Web Development with JavaScript

- [Web Developmentwith JS](#wdjs)
  - [Announcements](#announcements)
  - [Syllabus](./syllabus/WDJS.pdf)
  - [Schedule](#schedule)
  - [week](./syllabus/week.md)
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

| Week | Topic                                        | Activity & Assignment                                      |
|------|----------------------------------------------|------------------------------------------------------------|
| 1    | Computational Thinking                       | [Discusssions](https://docs.google.com/forms/d/e/1FAIpQLSewOHsYDaAqJHVzWkfybyMOfAs68FkDvHkmo91DjJfzmAsgyw/viewform),[Knowledge Check], [Coding Activity & Assignment] |
| 2    | Mental Model of Computing Operations         | Discusssions,Knowledge Check, Coding Activity & Assignment |
| 3    | Introduction to JavaScript                   | Discusssions,Knowledge Check, Coding Activity & Assignment |
| 4    | Functions: Array Manipulation And Scope      | Discusssions,Knowledge Check, Coding Activity & Assignment |
| 5    | Callback Functions                           | Discusssions,Knowledge Check, Coding Activity & Assignment |
| 6    | Introduction To GitHub, Testing, And The DOM | Discusssions,Knowledge Check, Coding Activity & Assignment |
| 7    | Styles And Bootstrap                         | Discusssions,Knowledge Check, Coding Activity & Assignment |
| 8    | Asynchronous Code                            | Discusssions,Knowledge Check, Coding Activity & Assignment |
| 9    | Introduction to Cyber Scurity and Recursion  | Discusssions,Knowledge Check, Coding Activity & Assignment |
| 10   | GitHub Portfolio Project                     | Discusssions,Knowledge Check, Coding Activity & Assignment |


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