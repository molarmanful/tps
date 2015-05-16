# Timer Program Starter
Javascript Rubik's Cube timer framework. Source includes jQuery, jQuery Cookie, Mark 2 (+Skewb), and jChester.

## Download
Include in head or body:
```html
<!--only include tps-scramblers.js if you need other WCA events besides 3x3x3-->
<script src="https://molarmanful.github.io/tps/tps-scramblers.js"></script>

<script src="https://molarmanful.github.io/tps/tps.js"></script>
```

## Usage
```js
var timer = new tps('.scramble', '.timer-display', ['333']); //initialize

//scrambling
timer.scramble(); //scramble
timer.event('333oh'); //change event - must be defined in initialization function

//timing
timer.inspect(15); //inspect (number value)
timer.start(); //start timer
timer.stop(); //stop timer

//stats
timer.times(); //get array of times for current event
timer.best(); //get session best time
timer.worst(); //get session worst time
timer.avg(5); //find last average of n
timer.mean(3); //find last mean of n

//time deleting
timer.delete(4); //delete time at specified index in time array
timer.resetall(); //delete all times for the event

//storage
timer.store(); //store times in local storage (or cookies if no local storage)
timer.recall(); //get times from local storage or (cookies if no local storage)
```
