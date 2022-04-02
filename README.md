# CSharp-inheritence

1) In c# it is possible to inherit fields and methods from one class to another
2) Categorised into two types

                    i) Derived Class(Child class)---Class that inherits from  another class
                    ii) Base Class(Parent Class)-----Class that being inherited

3)   To inherit from a class we use : symbol

# Why Inheritance

1)It is useful for code reusability(Re-use fields and methods of an existing class when you create a new class)
2)If we don't want a class to be inherted,use the "sealed" keyword.

========================

using System;

namespace Inheritance 
{

  // base class
  class Animal 
  { 

    public string name;

    public void display() 
    {
      Console.WriteLine("I am an animal");
    }
    
  } 
  
  // derived class of Animal 
  class Dog : Animal 
  {
    
    public void getName() 
    {
      Console.WriteLine("My name is " + name);
    }
  }

  class Program 
  {

    static void Main(string[] args)
    {

      // object of derived class
      Dog labrador = new Dog();

      // access field and method of base class
      labrador.name = "Dora";
      labrador.display();

      // access method from own class                            //ouput: I am an animal
                                                                          My name is Dora
      labrador.getName();

      Console.ReadLine();
    }

  }
}

===================================================

using System;

public class nani
{
    public string valentine="Christy";
}
public class Sajeev : nani
{
    public string pet="Dora";
}
class Sajeev
{
    public static void Main(string[]args)
    {
        Sajeev p = new Sajeev();
        Console.WriteLine("valentine:"+p.valentine);           //valentine:Christy
        Console.WriteLine("pet:"+p.pet);                      //pet:Dora
    }
}








6) 
