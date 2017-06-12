## Scope, hoisting and compartmentalization

### Answer the following:
In you own words, explain the concepts of scope, hoisting, compartmentalization.

scope: global scope/local scope
global scope= var assigns outside the function, and can be access everywhere
local scope= assign inside the function, can only be called inside the function.

hoisting:When the JavaScript interpreter executes your code, it will hoist all functions and variables to the top of their containing scope.

compartmentalization: a function used in JavaScript that runs right after being defined.
### Provide examples for all three, below:

#### Scope:
var pet = 'dog';

function printPet() {

  var otherPet = "cat";

  console.log(pet);
}

printPet();     

#### Hoisting:
function foo(){
    var bar;
    bar();
    bar = function(){

    };
}

foo();
#### Compartmentalization:
(function () {

var dog = 'poppy';
console.log(dog);

})();
