#JS Day 1 Homework

Go through each sample code and work out what the output will be and explain what happened.

### Episode 1
```js
var name = 'Keith';

var printName = function() {
  console.log('My name is ' + name );
};

printName();

It will print to the console 'My name is Keith'

```

### Episode 2
```js
score = 5;

var result = function() {
  var score = 3;
  return score;
};

console.log(result());

It will ignore the top score of 5 and print the variable inside the function, which is 3

```

### Episode 3
```js
var myAnimals = ['Chickens', 'Cats', 'Rabbits'];

var listAnimals = function() {
  myAnimals = ['Ducks', 'Dogs', 'Lions'];
  for(var i=0;i<myAnimals.length; i++){
    console.log(i + ": " + myAnimals[i]);
  }
}

listAnimals();

It will ignore the top myAnimals array and then print i which is the index of the array and then the item in that index place seperated by a colon. 

```

### Episode 4

```js
var suspectOne = 'Jay';
var suspectTwo = 'Val';
var suspectThree = 'Keith';
var suspectFour = 'Rick';

var allSuspects = function() {
  var suspectThree = 'Harvey'
  console.log('Suspects include: ' + suspectOne + ', ' + suspectTwo + ', ' + suspectThree + ', ' + suspectFour)
};

allSuspects();
console.log( 'Suspect three is:' + suspectThree );
```

first it will print Suspects include: the suspects with Harvey instead of Keith.
Then it will print Suspect three is Keith, because the Harvey replacement is inside the function.

### Episode 5

```js
var detective = {
  name : 'Ace Ventura',
  pet : 'monkey'
};

var printName = function(detective) {
  return detective.name
};

var detectiveInfo = function() {
  detective['name'] = 'Poirot'
  return printName(detective);
};

console.log(detectiveInfo());
```

It will print the detectiveInfo function which replaces the detective name to Poirot, so it will print Poirot.

### Episode 6
```js
var murderer = 'rick';

var outerFunction = function() {
  var murderer = 'marc';

  var innerFunction = function() {
    murderer = 'valerie';
  }

  innerFunction();
}

outerFunction();
console.log('the murderer is ', murderer);
```

print Valerie? I'm not sure actually, because Valerie is called by the innerFunction at the end of the outerFunction and then the OuterFunction is called. Could be Rick too....

### Episode 7 - Make up your own episode/s!

Make up your own episode which can be whatever you wish and the rest of the class will work out together what happened and what the output will be.


var wrestlers = [
  { name: 'AJ Styles',
    finisher: 'Styles Clash'
  },
  { name: 'The Miz',
    finisher: 'Skull Crushing Finale'
  },
  { name: 'Y2J',
    finisher: 'Code Breaker'
  },
]; 

var finisher;
for (var wrestler of wrestlers) {
  if (wrestler.name === 'Y2J') {
    finisher = wrestler.finisher;
  }
}

console.log(wrestlers[2]);





