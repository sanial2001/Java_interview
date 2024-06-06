- [**Multithreading**](https://www.interviewbit.com/multithreading-interview-questions/) is a Java feature that permits the execution of two or more portions of a program at the same time to maximise CPU efficiency. Each such portion of the program is referred to as a thread
- With the use of threads, we utilise multithreading and not multiprocessing, as they share same memory space and context switching between threads takes place very quickly as compared to processes
- We can instantiate thread in java using Java.Runnable or Thread Class
- Multithreading can be performed in Java using two different mechanisms:
	- By Extending the Thread class
	- By implementing the Runnable Interface

- **THREAD CLASS** 
	- We’ll make a class that extends the java.lang.Thread class. The run() method of the Thread class is overridden by this class. The run() procedure is where a thread starts its life. To begin thread execution, we construct an object of our new class and use the start() method. Start() calls the Thread object’s run() function.
	  ```java
			class Sample extends Thread {
			   public void run()
			   {
			       try {
			           System.out.println(
			               "Thread " + Thread.currentThread().getId()
			               + " is running");
			       }
			       catch (Exception e) {
			           System.out.println("An exception is caught");
			       }
			   }
			}
			
			class Multithread {
			   public static void main(String[] args)
			   {
			       int n = 5;
			       for (int i = 0; i < n; i++) {
			           Sample obj
			               = new Sample();
			           obj.start();
			       }
			   }
			} 
		```

- **RUNNABLE CLASS :**
	- We make a new class that implements the java.lang.Runnable interface and overrides the run() method. After that, we create a Thread object and call its start() method
	  ```java
	  class Sample implements Runnable {
		   public void run()
		   {
		       try {
		           System.out.println(
		               "Thread " + Thread.currentThread().getId()
		               + " is running");
		       }
		       catch (Exception e) {
		           System.out.println("An exception is caught");
		       }
		   }
		}
		
		class Multithread {
		   public static void main(String[] args)
		   {
		       int n = 5; 
		       for (int i = 0; i < n; i++) {
		           Thread obj
		               = new Thread(new Sample());
		           obj.start();
		       }
		   }
		} 
```

- **DIFFERENCE** :
	 1. Because Java doesn’t support multiple inheritances, if we extend the Thread class, we won’t be able to extend any other classes. Our class, however, can still extend other base classes if we implement the Runnable interface.
	 2. We can obtain rudimentary thread functionality by extending the Thread class, which has several built-in methods like yield() and interrupt() that aren’t available in the Runnable interface.
	 3. When you use runnable, you’ll get an object that can be shared by numerous threads