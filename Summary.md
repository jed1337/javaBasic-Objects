# Summary
## ExceptionTest
1. What is the knowledge point of the test? Where is the official document to the knowledge point?
	* How to create customised exceptions
	* Try with resources
	* How Java handles return statements in the finally block
	* How to handle nested exceptions
		* How to pass loggers between them
	* How to access stack trace elements
	* Official documents
		* [14.20.2. Execution of try-finally and try-catch-finally](https://docs.oracle.com/javase/specs/jls/se7/html/jls-14.html#jls-14.20.2)
		* [Try block](https://docs.oracle.com/javase/tutorial/essential/exceptions/try.html)
		* [Try with resources](https://docs.oracle.com/javase/tutorial/essential/exceptions/tryResourceClose.html)
		* [AutoCloseable](https://docs.oracle.com/javase/8/docs/api/java/lang/AutoCloseable.html)
		* [StackTraceElement](https://docs.oracle.com/javase/8/docs/api/java/lang/StackTraceElement.html)
2. Why the test failed at first?
	* The correct value wasn't there
3. Why you corrected the test that way?
		* should_customize_exception and should_customize_exception_continued
			* I called the constructor in the ```Exception``` from the ```StringFormatException```
		* should_get_method_name_in_stack_frame
			* I got the ```StackTraceElement``` of should_get_method_name_in_stack_frame.
			* I used the class name and method name
4. Do you have further questions on this knowledge point?
	* In what cases would you need to return a value in the finally block.
	* Since we have debuggers, what's a different application of accessing method names?

## InheritanceTest
1. What is the knowledge point of the test? Where is the official document to the knowledge point?
	* How a subclass calls its parent class's constructor
	* How overridden methods are called
	* Instantiating a parent class as one of its subclasses
		* You can't instantiate a subclass as its parent class
	* Casting
	* How ```instanceof``` works
	* ```Object#equals``` and ```Object#hashCode```
	* Official documents
		* [Inheritance](https://docs.oracle.com/javase/tutorial/java/IandI/subclasses.html)
		* [Overriding and Hiding Methods](https://docs.oracle.com/javase/tutorial/java/IandI/override.html)
		* [Upcasting, downcasting](https://www.cs.utexas.edu/~cannata/cs345/Class%20Notes/14%20Java%20Upcasting%20Downcasting.htm)
		* [The Type Comparison Operator instanceof](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/op2.html)
		* [equals](https://docs.oracle.com/javase/8/docs/api/java/lang/Object.html#equals-java.lang.Object-)
		* [hashCode](https://docs.oracle.com/javase/8/docs/api/java/lang/Object.html#hashCode--)
2. Why the test failed at first?
	* The correct value wasn't there
3. Why you corrected the test that way?
	* should_be_derived_from_object_class
		* should_call_super_class_constructor, should_call_super_class_constructor_continued, and should_call_super_class_constructor_more
			* I listed the order of the method calls
	* Tests involving ```Object#equals``` and ```Object#hashCode```
		* I used Intellij's code generator for that
4. Do you have further questions on this knowledge point?
	* None

## ObjectTest
1. What is the knowledge point of the test? Where is the official document to the knowledge point?
2. Why the test failed at first?
	* The correct value wasn't there
3. Why you corrected the test that way?
4. Do you have further questions on this knowledge point?
	* None

