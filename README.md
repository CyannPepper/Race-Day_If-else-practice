# Race-Day_If-else-practice
Simple program that helps runners register for a big race day. Made in JavaScript main.js under a codecademy project.

let raceNumber = Math.floor(Math.random() * 1000);

let registerEarly = true;
let runnerAge = 18

// checks if runner in an adult and registered early
if (runnerAge > 18 && registerEarly) {
  raceNumber += 1000;
}

// Displays time and number to early registered adults
if (runnerAge > 18 && registerEarly) {
  console.log('You are set to race at 9:30. You\'re number is: ' + raceNumber);
}

// displays time and number to late registered adults
if (runnerAge > 18 && !registerEarly) {
  console.log('Late adults run at 11:00 am. You\'re race number is: ' + raceNumber);
} 

// displays time and number for youth
if (runnerAge < 18) {
  console.log('Youth registrants run at 12:30 pm (regardless of registration). You\'re number is: ' + raceNumber);
} else if (runnerAge === 18) {
  console.log('Please see the registration desk.');
}
