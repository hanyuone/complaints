# Java

This is what I hate about Java:

- Ridiculous verbosity. This is obvious in the "Hello, World!" program:

  ```java
  package com.qwerpderp.helloworld;
  
  public class HelloWorld {
      public static void main(String[] args) {
          System.out.println("Hello, World!");
      }
  }
  ```
  
  All of this code, just to print out "Hello, World!" to the console. Python does it in one straightforward line:
  
  ```python
  print("Hello, World!")
  ```
  
  Why do you have to do this to me, Java?
  
- Terrible, terrible code from libraries. This is compounded by the verbosity thing. For example, this is a snippet of the sample code from LWJGL (Lightweight Java Game Library):

  ```java
  glfwSetKeyCallback(window, (window, key, scancode, action, mods) -> {
      if ( key == GLFW_KEY_ESCAPE && action == GLFW_RELEASE )
	  glfwSetWindowShouldClose(window, true);
  });
  
  /* some code later */
  
  GLFWVidMode vidmode = glfwGetVideoMode(glfwGetPrimaryMonitor());
  
  /* some more code later */
  
  while ( !glfwWindowShouldClose(window) ) {
  }
  ```
  
  This isn't funny, LWJGL. `glfwSetWindowShouldClose`? Seriously? I want to curl up into a ball and cry in my bed after seeing that. This probably isn't representative of the Java ecosystem, but LWJGL is a pretty big library. And Java devs, by some magical amount of willpower, deal with this.
