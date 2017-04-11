BT Angula

1. What is TypeScript and Why do we need it?
	TypeScript:  a language for application-scale JavaScript,convert ES6 about ES5
	Because: TypeScript is free,it  supports tools for large-scale JavaScript applications for any browser
2. How can you get TypeScript and install it?
	npm install -g typescript
3. How do you compile TypeScript files?
	tsc --watch base.ts base.js
4. Which Object Oriented terms are supported by TypeScript? Write an example.
	Inheritance:
```js
		class Animal {
		
		}
		class Dog extends Animal{
		}
	Abstract Classes:
		abstract class Animal {
   			 abstract makeSound(): void;
   			 move(): void {
       		 	console.log("roaming the earth...");
  		  	}
		}
```
5. How do you implement inheritance in TypeScript? Write an example.
	class Sports {
  	  private _name : string;
  	  constructor(name:string){
     	  this._name = name;
  	  }
	}
	class Soccer extends Sports {
  	  constructor(name:string){
        	 super(name);
   	 }
	}
```
CS6: Block scope variable
	var a = 1;

      function show() {
      alert(a);      }
	
	````
	emplate Literals:
	var name = 'dieu';

       console.log(`hello  ${name} `)
	````
	Multi-line strings
	var html = '<ul> <li> </li> </ul>'
	````
	For ..  of
	
	var list = ['one','two','three' ];
	for (let value of list){
	console.log(value);
	}
	Default parameters
	function append(value, array = []) {
  
      array.push(value);
       return array;
       }

    
	  append(1);
		
		
