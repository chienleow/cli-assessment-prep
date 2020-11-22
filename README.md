# CLI Assessment Prep 👨🏻‍💻 👩🏻‍💻

## Possible CLI Questions
**1. What is a gem?** _A packaged Ruby application or library_

**2. What is a shebang line? What does it do?** _It is telling us where to find the library we are going to use to run this code_
  
**3. What does require_relative do?** _Use require_relative when you are referring to a file that is relative to the current file you are working on (basically, within the same project directory)_
  
**4. Explain your executable file**

**5. Explain module, name-spacing, difference between class methods and instance methods?** 

**Example:** `EcommerceApp::CLI.new.start`

`EcommerceApp`**(a module)**: We need this to distinguish our CLI class from other modules if we have any

`CLI`**(a class)**

`.new`**(initialize)**: a **class method**, how do you tell? look at the receiver, which is the left to the dot "CLI.new"

`.start`: an **instance method**

`::`double colon, **name-spacing**, nested within the module of `EcommerceApp`

**Class method VS Instance method** [short read](https://dev.to/adamlombard/ruby-class-methods-vs-instance-methods-4aje)
- A method provides functionality to an Object
- Class method calls on the class, provides functionality to the CLASS itself
- Instance method calls on the instance OF the class, provides functionality to ONE instance of the class

**6. "self is implicit" meaning?**
- Every method you call is received by some object, the object receiving the method call is the receiver. 
- If you mention the object in the call, that's "explicit", if you call a method in the same object as the context without mentioning "self", that's "implicit".

**7. Truthy VS Falsey**
In Ruby only false and nil are falsey. Everything else is truthy (yes, even 0 is truthy).

## Ruby Essentials (From the checklist given)
**1. Basic control flow - how "if" statements work**
_Essentially check whether a condition is true or not_
2. Variable scopes - method, instance and class
	Scope refers to what variables are available at that time. 
	More info: Ruby Scopes
Instance Variables: Sharing data inside a Ruby object
Local Variables: The narrowest scope, defined inside the methods

3. Object instantiation - #new (and possibly #initialize)
	- We create a new instance of a class by calling the method new on that class, we also say that we “instantiate” that object
	- By calling Person.new we instantiate a new person object.
4. The meaning of the "self" keyword
	"Self" points to the object that "owns" the currently executing code
5. Method types - class vs. instance methods
	(look above)
6. Method return types - knowing what methods return
	Learn.co Puts, Print & Return
	The Differences Between Puts, Print & P
	Puts: Every message has its own line
	Print: Print without a newline
	P: shows a more “raw” version of an object
	Return: Return values
7. Iterating through collections - at least using #each with a block

 [] Extras
- Single Responsibility Principle
		API Class - bring in external API here, instantiate my objects
		Object Class (Listing/Category) - where objects are created and stored for user display
		CLI Class (Command Line Interface) - the controller of my app, communicates with my user, handle user input/output
- Separation of Concerns
- DRY code (Don't repeat yourself)
- Remember Object-Oriented: In Ruby, everything is an object.
