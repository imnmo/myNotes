### Java keywords and cheatsheet stuff

* instance variable and local variable
* int 32bits, long 64bits, float32bit, double 64bits
* object reference myClass myref = new myClass();
* what is **static initializer**?
	* The static initializer is a static {} block of code inside java class, and run only one time before the constructor or main method is called. 

    static
	{
	// do something
    }

* ***Interfaces*** can also be nested:
	* benefits:
		* It is a way of logically grouping interfaces that are only used in one place.
		* more readable and increses encapsulation
* eg: 
* 
		public interface Map {
		interface Entry{
			int getKey();
		}
		void clear();
		}



	