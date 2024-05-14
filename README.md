# Higher Order Functions and Iterators <br>

| Iterator Method | Descriiption of Iterator Method|
|---|---|
| array.forEach() | used to execute the same code on every element in an array but does not change the array and returns undefined. |
| array.map() | executes the same code on every element in an array and returns a new array with the updated elements. |
| array.filter() | checks every element in an array if it meets criteria and returns a new array with the elements meeting truthy for the criteria. |
| array.findIndex() | returns the index of the first element of an array that satisfies a condition in the callback function. It returns -1 if none of the elements in the array satisfies the condition. |
| array.reduce() | iterates through an array and takes the values of the elements and returns a single value. |
| All iterator methods take a callback function which makes them higher order functions  |
<br>

## HIGHER ORDER FUNCTIONS (HOF): <br>

------<br>
Take one or more functions as arguments, or returns a function as its result.<br>
// Callback function, passed as a parameter in the higher order function below:<br>

    function callbackFunction(){
          console.log('I am  a callback function');
     }
// higher order function<br>

    function higherOrderFunction(func){
         console.log('I am higher order function')
         func()
    }
// call the higher order function<br>

    higherOrderFunction(callbackFunction);
The above higher order functions take take a callback function as an argurment.<br>

    const arr = [1, 2, 3, 4, 5];
    const output = arr.map((num) => num += 10)
    console.log(arr); // [1, 2, 3, 4, 5]
    console.log(output); // [11, 12, 13, 14, 15]


