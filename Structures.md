# Structures
In C#, a structure is a value type data type. It helps you to make a single variable hold related data of various data
types. The struct keyword is used for creating a structure. 

Structures are used to represent a record. Suppose you want to keep track of your books in the library. You might want
to track the following attributes about each book:
  -Title
  -Author
  -Subject
  -Book ID
  
#Defining a Structure
To define a structure, you must use the struct statement.The struct statement defines a new data type, with more than
one member for your program.

For example, here is the way you can declare the Book structure:
  
       struct Books
        {
          public string title;
          public string author;
          public string subject;
          public int book_id;
        }
   
The following program shows the use the structure:


       using System;
       struct Books {
        public class testStructure {
         public static void Main(string[] args) { 
         Books Book1; /*Declare Book1 of type Book*/
         Books Book2; /*Declare Book2 of type Book*/
         
         /*book 1 specification*/
         Book1.title = "C Programming";
         Book1.author = "Nuha Ali";
         Book1.subject = "C Programming Tutorial";
         Book1.book_id = 6495407;
         
         /*book 2 specification*/
         Book2.title = "Telecom Billing";
         Book2.author = "Zara Ali";
         Book2.subject = "C Programming Tutorial";
         Book2.book_id = 6495700;
         
         /*Print Book1 Specification*/
         Console.WriteLine("Book 1 Title: {0}", Book1.title);
         Console.WriteLine("Book 1 Author: {0}", Book1.author);
         Console.WriteLine("Book 1 Subject: {0}", Book1.subject);
         Console.WriteLine("Book 1 Book Id: {0}", Book1.book_id);
         
         Console.ReadKey();
           }
         }
         
