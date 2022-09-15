# Content
- Clean Code

<hr/>

## Clean Code

### Clean Code
**Not Clean Code**
<br/>

![Not Clean Code](image/readme/Not%20Clean%20Code.PNG)
- A lot of code
- Hard to read
- A lot of deeply nested control structures

<br/>

![Not Clean Code - Comparison Function](image/readme/Not%20Clean%20Code%20-%20Comparison%20Function.PNG)
<br/>
def create(m, n) is a function which creates other functions (factory/higher-order function) and these other functions being created turns out to be validation functions (`lamda v: v < n` and `lambda v: v > n`)
<br/><br/>
We pre-configured them with a certain value (31). Then, we call the function to compare another value against the created value (`print(max(15))` and `print(max(32))`) where it checks the value either smaller or bigger depending on we chose max or min as a parameter for creating our validation function

- Code was very confusing
- Understanding what this code does will certainly take a couple of moments

<br/>

Clean Code is **not** about whether **code works**. Instead, it is about whether code is easy to read and understand.
<br/>
A vast majority of time is spent **reading and understanding** code. 
<br/>

**Clean Code - choose different names**
<br/>

![Clean Code - Comparison Function](image/readme/Clean%20Code%20-%20Comparison%20Function.PNG)

<br/>

**Clean Code - creating a class with good names (incl. validation logic)**
<br/>

![Clean Code - Comparison Function (2)](image/readme/Clean%20Code%20-%20Comparison%20Function%20(2).PNG)

### What is Clean Code
Clean Code is <u>easy to understand</u> - Dirty code is not.

- Should be <u>readable and meaningful</u>
- Should <u>reduce cognitive load</u>
- Should be <u>concise</u> and "to the point"
- Should <u>avoid unintuitive names</u>, <u>complex nesting</u> and <u>big code blocks</u>
- Should follow <u>common best practices</u> and patterns
- Should be <u>fun</u> to <u>write</u> and <u>to maintain</u>

### Write a Good Story
- Your code is <u>like an essay</u>
- You are the <u>author</u>
  - Write it such that it is fun and easy to read and understand

- **Key Pain Points**
    <br/>

    ![Clean Code - Good Story Key Pain Points](image/readme/Clean%20Code%20-%20Good%20Story%20Key%20Pain%20Points.PNG)

### Clean Code does not require strong typing
![Does not require strong typing](image/readme/Clean%20Code%20-%20Does%20not%20require%20strong%20typing.PNG)

### Functional vs OOP vs Procedural & Core Principles
![Clean Code - Functional vs OOP vs Procedural](image/readme/Clean%20Code%20-%20Functional%20vs%20OOP%20vs%20Procedural.PNG)

<br/>

![Clean Code - Core Principles](image/readme/Clean%20Code%20-%20Core%20Principles.PNG)

### Clean Code and Patterns & Principles
![Clean Code - Patterns and Principles](image/readme/Clean%20Code%20-%20Patterns%20and%20Principles.PNG)

### Clean Code vs Clean Architecture
![Clean Code - Clean Code vs Clean Architecture](image/readme/Clean%20Code%20-%20Clean%20Code%20vs%20Clean%20Architecture.PNG)

### Clean Code is written over time
![Clean Code - Clean Code is written over time](image/readme/Clean%20Code%20-%20Clean%20Code%20is%20written%20over%20time.PNG)

### How to write Clean Code
![Clean Code - How to write Clean Code](image/readme/Clean%20Code%20-%20How%20to%20write%20Clean%20Code.PNG)

### Embrace Refactoring
![Clean Code - Embrace Refactoring](image/readme/Clean%20Code%20-%20Embrace%20Refactoring.PNG)

### Clean Code vs Quick Code
![Clean Code - Clean Code vs Quick Code](image/readme/Clean%20Code%20-%20Clean%20Code%20vs%20Quick%20Code.PNG)

### Module & Course Resources
https://github.com/academind/clean-code-course-code/tree/general-resources

<hr/>

## Naming - Assigning Names to Variables, Functions, Classes & More

### Assigning Good Names
- **Naming "Things"**
  - Variables, Constants and Properties
  - Functions and Methods
  - Classes

- Names should be **meaningful**

<br/>

**Bad Naming Example**
<br/>

![Naming - Not Clear Naming](image/readme/Naming%20-%20Not%20Clear%20Naming.PNG)
- What are we doing here? 
  - What is MainEntity?
  - What does process do?
  - What is the value of login (function for which existence we check/boolean value/a string/error)

<br/>

**Bad Naming Example Fix - Readable and very easy to understand**
<br/>

![Naming - Not Clear Naming Solution](image/readme/Naming%20-%20Not%20Clear%20Naming%20Solution.PNG)
- Same code but it is way clearer (Picking good names really matters)
  - It is now obvious that we are creating a user
  - Then, save maybe to a file/database
  - isLoggedIn instead of login making it clear that this likely holds the result of checking whether the user is logged in or not (Boolean value - true/false)

### Why Names Matter
https://github.com/academind/clean-code-course-code/tree/naming-01-why-good-names-matter

<br/>

![Naming - Why Names Matter](image/readme/Naming%20-%20Why%20Names%20Matter.PNG)

### Names we might not always agree
![Naming - Names we might not always agree](image/readme/Naming%20-%20Names%20we%20might%20always%20not%20agree.PNG)

### How to name things correctly
![Naming- How to name things correctly](image/readme/Naming%20-%20How%20to%20name%20things%20correctly.PNG)

### Name Casing
![Naming - Name Casing](image/readme/Naming%20-%20Name%20Casing.PNG)

### Naming Variables, Constants & Properties
![Naming - Naming Variables, Constants and Properties](image/readme/Naming%20-%20Name%20Variables,%20Constants%20and%20Properties.PNG)

- **Variables Example**
    <br/>
    ![Naming - Variables Example](image/readme/Naming%20-%20Variables%20Example.PNG)

    <br/>

    ![Naming - Variables Example (2)](image/readme/Naming%20-%20Variables%20Example%20(2).PNG)
    <br/>
    - user entered in some form and we have a mixture of entered values and of validation results of us validating these inputs

    <br/>

    ![Naming - Variables Example (3)](image/readme/Naming%20-%20Variables%20Example%20(3).PNG)
    <br/>
    - user data variable holds this bag of entered values and validation results (would not be finished user object but intermediate object between collecting values and creating user)

### Naming Functions & Methods
![Naming - Naming Functions and Methods](image/readme/Naming%20-%20Naming%20Functions%20and%20Methods.PNG)

- **Naming Functions and Methods Example**
    <br/>
    ![Naming - Naming Functions and Methods Example](image/readme/Naming%20-%20Naming%20Functions%20and%20Methods%20Example.PNG)

    <br/>

    ![Naming - Naming Functions and Methods Example (2)](image/readme/Naming%20-%20Naming%20Functions%20and%20Methods%20Example%20(2).PNG)
    <br/>
    - it could be anything so this is definitely very unspecific and not the naming you wanna use 

    <br/>

    ![Naming - Naming Functions and Methods Example (3)](image/readme/Naming%20-%20Naming%20Functions%20and%20Methods%20Example%20(3).PNG)
    <br/>
    - if save is a method on a user object, then its way clearer and then save is perfectly fine
    - but if you just have a function called save, which is not called on an object yet receives an object as an argument, there might be a better name which you can choose (e.g. saveUser)

    <br/>

    ![Naming - Naming Functions and Methods Example (4)](image/readme/Naming%20-%20Naming%20Functions%20and%20Methods%20Example%20(4).PNG)
    <br/>
    - throwing an error if validation fails (e.g. isValid is great name if function returns true or false)

### Naming Classes
![Naming - Naming Classes](image/readme/Naming%20-%20Naming%20Classes.PNG)

- **Naming Classes Example**
    <br/>
    ![Naming - Naming Classes Example](image/readme/Naming%20-%20Naming%20Classes%20Example.PNG)

### Exceptions we should be aware of
https://github.com/academind/clean-code-course-code/tree/naming-02-naming-exceptions

<br/>

![Naming- Exceptions we should be aware of](image/readme/Naming%20-%20Exceptions%20we%20should%20be%20aware%20of.PNG)
- Python code snippet using the date time library (Python standard library - built-in module)
- `datetime.now()` to get the current timestamp of today, giving us a date object which then can be formatted to a string with certain formatting rules by using strftime method (`date_today.strftime('%Y=%m=%d')`)
- these names violate the naming conventions but it is a method and not a property and since it is a built-in library, you can't change or override it

<br/>

![Naming- Exceptions we should be aware of (2)](image/readme/Naming%20-%20Exceptions%20we%20should%20be%20aware%20of%20(2).PNG)
- database clause (`private client: any;`) has a private property client, which is actually set when the connect method is called (`this.client = {}`)
- however, since that property is private, it cannot be accessed from outside the class, instead we have this connected client getters (`get connectedClient()`) - access like a property through `db.connectedClient.query();`
- getters and setters are a special concepts exist in multiple programming languages to provide us as a developer with greater control over how data in a class can be read or set (it is okay to use property naming rules for getters and setters)
  - a getter method allows us to control access to certain properties in the class

### Common Errors & Pitfalls
- **Do not include redundant information in Names**
    <br/>
    ![Naming - Do not include redundant information in Names](image/readme/Naming%20-%20Do%20not%20include%20redundant%20information%20in%20Names.PNG)

- **Avoid slang, unclear abbreviations and disinformation**
    <br/>
    ![Naming - Avoid slang, unclear abbreviations and disinformation](image/readme/Naming%20-%20Avoid%20slang,%20unclear%20abbreviations%20and%20disinformation.PNG)

- **Choose distinctive Names**
    <br/>
    ![Naming - Choose distinctive Names](image/readme/Naming%20-%20Choose%20distinctive%20Names.PNG)

- **Be Consistent**
    <br/>
    ![Naming - Be Consistent](image/readme/Naming%20-%20Be%20Consistent.PNG)
    <br/><br/>
    ![Naming - Be Consistent (2)](image/readme/Naming%20-%20Be%20Consistent%20(2).PNG)
        - if you went with `get_users` in one place and use `get_products` in another place, don't have `fetch_products` in one class and `get_users` in another class (it will not be obvious if these methods do generally the same thing/there is a key difference between getting and fetching in our program)

### Demo
https://github.com/academind/clean-code-course-code/tree/naming-03-demo

### Challenge - Problem & Solution
https://github.com/academind/clean-code-course-code/tree/naming-04-challenge

### Module Resources
https://github.com/academind/clean-code-course-code/tree/naming-extra-attachments

<hr/>

## Code Structure, Comments & Formatting

### Bad Comments
https://github.com/academind/clean-code-course-code/tree/comments-formatting-01-bad-comments

<br/>

![Code Structure - Bad Comments](image/readme/Code%20Structure%20-%20Bad%20Comments.PNG)

- **Redundant Information**
    <br/>
    ![Code Structure - Bad Comments (2)](image/readme/Code%20Structure%20-%20Bad%20Comments%20(2).PNG)
    - Use dbEngine instead of dbDriver
    
    <br/>

    ![Code Structure - Bad Comments (3)](image/readme/Code%20Structure%20-%20Bad%20Comments%20(3).PNG)
    - if we use proper names like in this example, you should not need any explanatory comments (sometimes comments makes it hard to understand)

- **Dividers/Block Markers**
    <br/>
    ![Code Structure - Bad Comments (4)](image/readme/Code%20Structure%20-%20Bad%20Comments%20(4).PNG)
    - inform developers going through this code file that we are defining a couple of globals and classes (this should be obvious - do not need to define as we can tell by the class keyword)

- **Misleading Comments**
    <br/>
    ![Code Structure - Bad Comments (5)](image/readme/Code%20Structure%20-%20Bad%20Comments%20(5).PNG)
    - we say that we are updating a user but actually the name implies that we are inserting a user which is not the same as updating (comment does not help us at all)
    - if we can't rename the method because of some badly written third-party library, we should at least update the comment to something like `update a user, although the method name says "insert"` to make it clear that comment is right and not the method (best is to rename method)

- **Commented-Out Code**
    <br/>
    ![Code Structure - Bad Comments (6)](image/readme/Code%20Structure%20-%20Bad%20Comments%20(6).PNG)
    - if we have codes that we do not use anymore, we should just remove it
    - nowadays, we should be using version control systems like Git and therefore we can always bring back deleted code if we really need it

### Good Comments
https://github.com/academind/clean-code-course-code/tree/comments-formatting-02-good-comments

<br/>

![Code Structure - Good Comments](image/readme/Code%20Structure%20-%20Good%20Comments.PNG)

**Avoid Comments** with only very few exceptions such as:
- **Legal Information**
    <br/> 
    ![Code Structure - Good Comments (2)](image/readme/Code%20Structure%20-%20Good%20Comments%20(2).PNG)
    - Code has such a legal disclaimer/comment right at the top (depending on project, we might need to add something like this to every code file)

- **Explanations which cannot be replaced by good naming**
    <br/> 
    ![Code Structure - Good Comments (3)](image/readme/Code%20Structure%20-%20Good%20Comments%20(3).PNG)
    - Using a regular expression can get quite long and having a little comment explains what does it do/checks for can be worth a lot

- **Warnings**
    <br/> 
    ![Code Structure - Good Comments (4)](image/readme/Code%20Structure%20-%20Good%20Comments%20(4).PNG)
    - A comment warning us that this specific API (local storage API) is only available in JavaScript running in the browser, not running on the number of machine with NodeJS

- **Todo Notes**
    <br/> 
    ![Code Structure - Good Comments (5)](image/readme/Code%20Structure%20-%20Good%20Comments%20(5).PNG)
    - if we do have some code which is unfinished, adding a Todo note comment like this can indeed make sense and be okay (should not overdo it and should focus on writing code which you finish instead of leaving unfinished code)
    
    <br/>

    ![Code Structure - Good Comments (6)](image/readme/Code%20Structure%20-%20Good%20Comments%20(6).PNG)
    - add documentation especially when providing a public API

### Code Formatting 
![Code Structure - Code Formatting](image/readme/Good%20Structure%20-%20Code%20Formatting.PNG)

### Proper Formatting
![Code Structure - Proper Formatting](image/readme/Good%20Structure%20-%20Proper%20Formatting.PNG)

<br/>

Note: Simply search for "[LANGUAGE] style guide" - e.g. "Python style guide" will yield the PEB8 style guide documentation

### Veritical Formatting
https://github.com/academind/clean-code-course-code/tree/comments-formatting-03-vertical-formatting

<br/>

![Code Structure - Vertical Formatting](image/readme/Good%20Structure%20-%20Vertical%20Formatting.PNG)

- Should have blank lines (create vertical space - makes the code more readable)

<br/>

Note: Modern IDEs offer autoformatting tools and shortcuts - even adjusted to language-specific conventions
<br/>
https://github.com/academind/clean-code-course-code/tree/comments-formatting-04-language-specific
- For Python, you cannot call function before it was to find while for JavaScript, you can

### Horizontal Formatting
![Code Structure - Horizontal Formatting](image/readme/Good%20Structure%20-%20Horizontal%20Formatting.PNG)

### Challenge - Problem & Solution
https://github.com/academind/clean-code-course-code/tree/comments-formatting-05-challenge

### Module Resources
https://github.com/academind/clean-code-course-code/tree/comments-formatting-extra-attachments

<hr/>

## Functions & Methods

### What makes up a Function
![Functions Methods - What makes up a Function](image/readme/Functions%20Methods%20-%20What%20makes%20up%20a%20Function.PNG)

- **Calling a function and with passing values for function parameters**
  - **Minimize** the number of parameters
    <br/>
    ![Functions Methods - Number of parameters](image/readme/Functions%20Methods%20-%20Number%20of%20parameters.PNG)

    <br/>
    https://github.com/academind/clean-code-course-code/tree/functions-01-refactoring-function-parameters
    <br/>
      
      - Refactoring Function Parameters (Ideas and Concepts)
        <br/>
        
        ![Funtions Methods - Refactoring Function Parameters](image/readme/Functions%20Methods%20-%20Refactoring%20Function%20Parameters.PNG)
          - this function only takes one argument (already finished user)
       
        <br/>

        ![Funtions Methods - Refactoring Function Parameters (2)](image/readme/Functions%20Methods%20-%20Refactoring%20Function%20Parameters%20(2).PNG)
          - it is easier to understand and call, does not leave us guessing whether email/password should be first and which kind of values this function might want

        <br/>

        ![Funtions Methods - Refactoring Function Parameters (3)](image/readme/Functions%20Methods%20-%20Refactoring%20Function%20Parameters%20(3).PNG)
          - a class user which acts as a blueprint for a new user objects, has a safe method which can be called without any arguments. Therefore, `user.safe` is very easy to read and very clear and understandable (pass email/password to user constructor function)