In C#, you can use strings as an array of characters. However, more common practice is to use the string keyword 
to declare a string variable. The string keyword is an alias for the System.String class.

#Creating a String Object
You can create string object using one of the following methods:
-By assigning a string literal to a String variable
-By using a String class constructor
-By using the string concatenation variable +
-By retrieving a property or calling a method that returns a string
-By calling a formatting method to convert a value or an object to its string representation

         using System;
         namespace String Application {
          class Program {
           static void Main(string[] args) {
            //from string literal and string concatenation
            string fname, lname;
            fname = "Rowan";
            lname = "Atkinson";
            
            string fullname = fname + lname;
            Console.WriteLine("Full Name: {0}", fullname);
            
            //by using string constructor
            char[] letters= {'H', 'e', 'l', 'l', 'o'};
            string greetings = new string(letters);
            Console.WriteLine("Greetings: {0}", greetings);
            
            //methods returning string
            string[] sarray = {"Hello", "From", "Tutorials", "Point"};
            string message = String.Join("", sarray);
            Console.WriteLine("Message: {0}", message);
            
            //formatting method to convert a value
            DateTime waiting = new DateTime(2012, 10, 10, 17, 58, 1);
            string chat = String.Format("Message sent at {0:t} on {0:D}";
            Console.WriteLine("Message: {0}", chat);
