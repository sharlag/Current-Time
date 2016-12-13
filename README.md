# Current-Time

Using JavaScript to display the current time numerically. 

```bash
var clockID = 0;
function UpdateClock() {
   if(clockID) {
    clearTimeout(clockID);
    clockID  = 0;
   }
      var tDate = new Date();
      document.theClock.theTime.value = "" 
         + tDate.getHours() + ":" 
         + tDate.getMinutes() + ":" 
         + tDate.getSeconds();
      clockID = setTimeout("UpdateClock()", 1000);
      }
function StartClock() {
   clockID = setTimeout("UpdateClock()", 500);
}
function KillClock() {
   if(clockID) {
      clearTimeout(clockID);
      clockID  = 0;
   }
}
```

Current-Time/ss.png
<img src="https://sharlag.github.io/Cat-Walk/images/catwalk.gif" alt="Image of moving cat">
