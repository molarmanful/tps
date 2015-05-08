# Timer Program Starter
Javascript Rubik's Cube timer framework. Source includes jQuery, jQuery Cookie, and Mark 2 3x3 scrambler.

## Download
The code is hosted at http://molarmanful.github.io/tps/tps.js. Include that script in your head tag.

## Usage
```js
var timer = new tps('.scramble', '.timer-display', ['333']); //initialize
timer.scramble(); //scramble
timer.event('333oh'); //change event - must be defined in initialization function
timer.inspect(15); //inspect (number value)
timer.start(); //start timer
timer.stop(); //stop timer
timer.times(); //get array of times for current event
timer.avg(5); //find last average of n
timer.mean(3); //find last mean of n
timer.store(); //store times in local storage (or cookies if no local storage)
timer.recall(); //get times from local storage or (cookies if no local storage)
```
