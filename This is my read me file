How to compare two JSON have the same properties without order?
 a. let obj1 = { name: "Person 1", age:5};
b. let obj2 = { age:5, name: "Person 1" };

let obj1 = { name: "Person 1", age: 5 };
let obj2 = { age: 5, name: "Person 1" };

let obj1String = JSON.stringify(obj1);
let obj2String = JSON.stringify(obj2);

let sortedObj1String = obj1String.split('').sort().join('');
let sortedObj2String = obj2String.split('').sort().join('');

if (sortedObj1String === sortedObj2String) {
  console.log("The JSON objects have the same properties (ignoring order).");
} else {
  console.log("The JSON objects have different properties (ignoring order).");
}

2, Use the rest countries' API URL -> https://restcountries.com/v3.1/all and display all the country I
flags in the console.

fetch("https://restcountries.com/v3.1/all")
  .then(response => response.json())
  .then(data => {
    // Iterate over each country in the response data
    data.forEach(country => {
      // Check if the country has a flag property
      if (country.flags) {
        console.log(country.flags.png); // Display the flag URL in the console
      }
    });
  })
  .catch(error => {
    console.log("An error occurred while fetching the data:", error);
  });
