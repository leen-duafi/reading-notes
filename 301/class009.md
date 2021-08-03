**What is functional programming?**

 is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data 

**What is a pure function and how do we know if something is a pure function?**

pure functions are stable, consistent, and predictable. Given the same parameters, pure functions will always return the same result. We don’t need to think of situations when the same parameter has different results — because it will never happen.

* It returns the same result if given the same arguments (it is also referred as deterministic)
* It does not cause any observable side effects

**What are the benefits of a pure function?**

 he code’s definitely easier to test. We don’t need to mock anything. So we can unit test pure functions with different contexts:


* Given a parameter A → expect the function to return value B
* Given a parameter C → expect the function to return value D

**What is immutability?**

Unchanging over time or unable to be changed.

When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

**What is Referential transparency?**
This pure function will always have the same output, given the same input.
pure functions + immutable data = referential transparency


**What is a module?**

split the code 
so we have differnt model for differnt code which has a certain functionlty on the application
then we call on them whenever we need them 
and it is essationally another java script file 

**What does the word ‘require’ do?**

global object in nofg so we can use it wherver we are

**How do we bring another module into the file the we are working in?**

require('/modelName')
models.export = {whatever we want to be avaiable outside }

**What do we have to do to make a module available?**

require('/modelName')
models.export = {whatever we want to be avaiable outside }
