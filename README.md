# know-your-console-log
Small documentation of few under-used console functions. [Full Spec](https://console.spec.whatwg.org/)

## console.table

Print objects nicely in tabular format.

```
console.table(window.location)
```

<img width="1283" alt="Screenshot showcasing output of console.table function" src="https://user-images.githubusercontent.com/1001829/92951031-5906e400-f47b-11ea-80a9-1a883081201a.png">

[MDN Link](https://developer.mozilla.org/en-US/docs/Web/API/Console/table)


## console.count

A count function for logging things like - how many times was a function called with a particular argument etc.

```
let user = "";

function greet() {
  console.count(user);
  return "hi " + user;
}

user = "bob";
greet();
user = "alice";
greet();
greet();
console.count("alice");
```

<img width="384" alt="Screenshot showcasing output of console.count function" src="https://user-images.githubusercontent.com/1001829/92951579-3628ff80-f47c-11ea-8606-33fa0d4b2e1c.png">

[MDN Link](https://developer.mozilla.org/en-US/docs/Web/API/Console/count)

## console.clear

Use this before printing if you expect the console to be cluttered when logging your particular line

## console.group

TBA

## console.time, console.timeEnd, console.timeLog

TBA
