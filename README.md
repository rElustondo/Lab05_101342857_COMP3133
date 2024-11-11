🚀 Exercise 1: Greeter Function
📄 Description
A simple JavaScript function that greets a user by their first and last name using an arrow function.

📝 Code
javascript
Copy code
let greeter = (firstname, lastname) => {
    console.log(`Hello ${firstname} ${lastname}`);
}

greeter("John", "Smith");
🖨️ Expected Output
Copy code
Hello John Smith
💡 Explanation
The greeter function takes two parameters: firstname and lastname.
It logs a greeting message to the console using template literals.
🛠️ Technologies Used
JavaScript (ES6 arrow functions)
📦 How to Run
To execute this code, save it to a .js file and run it using Node.js:

bash
Copy code
node greeter.js

🚀 Exercise 2: Customer Class
📄 Description
A simple TypeScript class named Customer that includes properties for first and last names, along with a method to greet the customer.

📝 Code
typescript
Copy code
class Customer {
    firstName: string;
    lastName: string;

    public greeter() {
        console.log(`Hello ${this.firstName} ${this.lastName}!`);
    }
}

let customer = new Customer();
customer.firstName = "Tom";
customer.lastName = "Hanks";
customer.greeter();
🖨️ Expected Output
Copy code
Hello Tom Hanks!
💡 Explanation
The Customer class has two properties: firstName and lastName, both of type string.
The greeter() method logs a greeting message to the console using the values of firstName and lastName.
An instance of the Customer class is created, and the firstName and lastName properties are set before calling the greeter() method.
🛠️ Technologies Used
TypeScript: A statically typed superset of JavaScript.
📦 How to Run
To compile and run this TypeScript code:

Save it in a file named customer.ts.
Compile it using the TypeScript compiler:
bash
Copy code
tsc customer.ts
Run the compiled JavaScript file:
bash
Copy code
node customer.js
⚠️ Note
Make sure you have TypeScript installed globally. If not, you can install it using:

bash
Copy code
npm install -g typescript


🚀 Exercise 3: Customer Class with Constructor and Private Properties
📄 Description
This TypeScript example demonstrates a class Customer with private properties and a constructor for initializing the customer's first and last names.

📝 Code
typescript
Copy code
class Customer {
    private firstName: string;
    private lastName: string;

    constructor(firstName: string, lastName: string) {
        this.firstName = firstName;
        this.lastName = lastName;
    }

    public greeter() {
        console.log(`Hello ${this.firstName} ${this.lastName}!`);
    }
}

let customer = new Customer("John", "Doe");
customer.greeter();
🖨️ Expected Output
Copy code
Hello John Doe!
💡 Explanation
The Customer class has two private properties: firstName and lastName, which are initialized through the constructor.
The constructor takes two parameters, firstName and lastName, and assigns them to the private properties.
The greeter() method logs a greeting message using the values of firstName and lastName.
An instance of the Customer class is created with specific values for firstName and lastName, and the greeter() method is called.
🛠️ Technologies Used
TypeScript: A statically typed superset of JavaScript with private class properties.
📦 How to Run
To compile and run this TypeScript code:

Save it in a file named customer.ts.
Compile it using the TypeScript compiler:
bash
Copy code
tsc customer.ts
Run the compiled JavaScript file:
bash
Copy code
node customer.js
⚠️ Note
Make sure you have TypeScript installed globally. If not, you can install it using:

npm install -g typescript

🚀 Exercise 4: Customer Class with Constructor, Private Properties, and Methods
📄 Description
This TypeScript exercise extends the previous example by adding an additional private property age to the Customer class. It includes methods for greeting and retrieving the customer's age.

📝 Code
typescript
Copy code
export class Customer {
    private firstName: string;
    private lastName: string;
    private age: number;

    constructor(firstName: string, lastName: string, age: number) {
        this.firstName = firstName;
        this.lastName = lastName;
        this.age = age;
    }

    public greeter() {
        console.log(`Hello ${this.firstName} ${this.lastName}!`);
    }

    public GetAge() {
        console.log(`Age: ${this.age}`);
        return this.age;
    }
}

import { Customer } from "./customer";

let customer = new Customer("Tom", "Hanks", 30);
customer.greeter();
customer.GetAge();
🖨️ Expected Output
makefile
Copy code
Hello Tom Hanks!
Age: 30
💡 Explanation
The Customer class has three private properties: firstName, lastName, and age.
The constructor is used to initialize all three properties when a new instance of the Customer class is created.
The greeter() method outputs a greeting message with the customer's name.
The GetAge() method logs the customer's age and returns it.
An instance of the Customer class is created with the name "Tom Hanks" and age 30, then the greeter() and GetAge() methods are called.
🛠️ Technologies Used
TypeScript: Used for type safety and class-based object-oriented programming.
📦 How to Run
To compile and run this TypeScript code:

Save it in a file named customer.ts.
Compile it using the TypeScript compiler:
bash
Copy code
tsc customer.ts
Run the compiled JavaScript file:
bash
Copy code
node customer.js
⚠️ Note
Ensure TypeScript is installed globally:

bash
Copy code
npm install -g typescript
