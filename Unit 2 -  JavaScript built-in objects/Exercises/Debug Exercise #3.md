# Debugging Practice
1. Fix syntax errors first. Run the following code as-is and read the error message. Fix the mistake, and then re-run the code to check it.
```javascript
let launchReady = false;
let fuelLevel = 17000;

if (fuelLevel >= 20000 {
   console.log('Fuel level cleared.');
   launchReady = true;
} else {
   console.log('WARNING: Insufficient fuel!');
   launchReady = false;
}
```

2. The next block of code hides two syntax errors. Run the code as-is to find the mistakes.
```javascript
let launchReady = false;
let crewStatus = true;
let computerStatus = 'green';

if (crewStatus &&& computerStatus === 'green') {
   console.log('Crew & computer cleared.');
   launchReady = true;
} else {
   console.log('WARNING: Crew or computer not ready!');
   launchReady = false;
}

if (launchReady) {
   console.log(("10, 9, 8, 7, 6, 5, 4, 3, 2, 1...");
   console.log("Fed parrot...");
   console.log("Ignition...");
   console.log("Liftoff!");
} else {
   console.log("Launch scrubbed.");
}
```

3. Fix runtime errors next. Remember to examine the error message for clues about what is going wrong. Pay close attention to any line numbers mentioned in the message - these will help you locate and repair the mistake in the code.
```javascript
let launchReady = false;
let fuelLevel = 17000;

if (fuellevel >= 20000) {
   console.log('Fuel level cleared.');
   launchReady = true;
} else {
   console.log('WARNING: Insufficient fuel!');
   launchReady = false;
}
```
