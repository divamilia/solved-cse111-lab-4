Download Link: https://assignmentchef.com/product/solved-cse111-lab-4
<br>
Trace the output of the following Java Codes. Then run them in Dr. Java to see if the results match.




<h1>Task 1</h1>

//Run the methodA() and methodB() on an Instance of Test few times and explain the answer.




public class Test{ int sum;

public int y; public void methodA(){ int x=0, y =0;     y = y + 7;     x = y + 11; sum = x + y;

System.out.println(x + ” ” + y+ ” ” + sum);

}

public void methodB(){ int x = 0;     y = y + 11;     x = x + 33 + y; sum = sum + x + y;

System.out.println(x + ” ” + y+ ” ” + sum);

} }




<h1>Task 2</h1>




public class Q3

{   public static void main(String args[])

{

String test = “”; int i = 5, j = 0, k = 15; while (i&lt; 10){    k-=1; j = k; while (j &gt; 10 ){ if (j % 2 == 0){ test = “&lt;–“;

test =  test + i + 2 + “–&gt;” + (j / 2);

} else { test = “–&gt;”;

test =  “–&gt;” + (i / 2) + test + j;

}

System.out.println(test);

–j;

}

i++;

}

}




<h1>Task 3</h1>




//Run the methodA() on an Instance of Test3 five times and explain the answer.




public class Test3{ public int sum; public int y;




public void methodA(){ int x=2, y =3; int [] msg = new int[1]; msg[0] = 3; y = this.y + msg[0]; methodB(msg, msg[0]); x = this.y + msg[0]; sum = x + y + msg[0];

System.out.println(x + ” ” + y+ ” ” + sum);

}




private void methodB(int [] mg2, int mg1){ int x = 0; y = this.y + mg2[0]; x = x + 33 + mg1; sum = sum + x + y; mg2[0] = y + mg1; mg1 = mg1 + x + 2;

System.out.println(x + ” ” + y+ ” ” + sum);

} }




<h1>Task 4</h1>

//Run the methodA() on an Instance of Test4 five times and explain the answer.




public class Test4{ public int sum; public int y;




<table width="0">

 <tbody>

  <tr>

   <td colspan="2" width="628">public void methodA(){</td>

  </tr>

  <tr>

   <td rowspan="2" width="48"></td>

   <td width="580">int x=0, y =0;</td>

  </tr>

  <tr>

   <td width="580">int [] msg = new int[1];</td>

  </tr>

 </tbody>

</table>

msg[0] = 5; y = y + methodB(msg[0]); x = y + methodB(msg, msg[0]); sum = x + y + msg[0];

System.out.println(x + ” ” + y+ ” ” + sum);

}

<table width="0">

 <tbody>

  <tr>

   <td colspan="2" width="628">Private int methodB(int mg2[] , int mg1){</td>

  </tr>

  <tr>

   <td width="48"></td>

   <td width="580">int x = 0;</td>

  </tr>

 </tbody>

</table>

y = y + mg2[0]; x = x + 33 + mg1; sum = sum + x + y; mg2[0] = y + mg1; mg1 = mg1 + x + 2;

System.out.println(x + ” ” + y+ ” ” + sum); return sum;

}




<table width="0">

 <tbody>

  <tr>

   <td width="628">private int methodB(int mg1){</td>

  </tr>

  <tr>

   <td width="628">int x = 0; int y = 0;</td>

  </tr>

 </tbody>

</table>

y = y + mg1;     x = x + 33 + mg1; sum = sum + x + y; this.y = mg1 + x + 2;

System.out.println(x + ” ” + y+ ” ” + sum); return y;

} }




<h1>Task 5</h1>




//What is the output if you execute the methodA( ) on an instance of the Test04 Class?




public class Test4{ public int sum; public int y; public void methodA(){     int x=0; int z = 0; while (z &lt; 5){       y = y + sum;        x = y + 1;

System.out.println(x + ” ” + y+ ” ” + sum); sum = sum + methodB(x, y);       z++;

}

}

public int methodB(int m, int n){ int x = 0; int sum = 0;     y = y + m;     x = n – 4;

sum = sum + y;

System.out.println(x + ” ” + y+ ” ” + sum);   return sum;

} }




<h1>Task 6</h1>




/* What is the output for the following code sequence? FinalT3A fT3A = new FinalT3A(); fT3A.methodA();

fT3A.methodB(6,8);

*/




public class FinalT3A{ public int sum; public int y;










public void methodA(){     int x=0, y =0, j = 0;  while (j &lt; 2){       y = y + j;        x = j + methodB(y , j); sum = x + y;

System.out.println(x + ” ” + y+ ” ” + sum); j++;

}   }

public int methodB(int p, int k){ int x = 0;     y = y + k + 1;     x = x + 3 – p; sum = sum + x + y;

System.out.println(x + ” ” + y+ ” ” + sum);   return sum;

} }

<h1>Task 7</h1>




class PuzzleTester{ public static void main(String[]args) {

Puzzle p = new Puzzle();

p.methodA();

p.methodA(); p=new Puzzle(); p.methodA();

p.methodB(7);

} }




class Puzzle {  static int x;

void methodA(){

int z;

x=5; //at home, comment/delete this line and try again  z=x+methodB(x);

System.out.println(x+” “+z);  z=methodB(z+2)+x;

System.out.println(x+” “+z); methodB(x,z); System.out.println(x+” “+z);

}

int methodB(int y){              x=y+x;

System.out.println(x+” “+y);

return x+3;

}

void methodB(int z, int x){

z=z+1;                   x=x+1;

System.out.println(z+” “+x);

}

}




<strong><u>Task 7.1</u></strong> class PuzzleTester{

public static void main(String[]args)

{

Puzzle p = new Puzzle();     p.methodA();

p.methodB(7);

}

}




class Puzzle{   static int x;

void methodA(){

int z;

x=5; //at home, comment/delete this line and try again

z=x+methodB(x);     Maze m1 = new Maze();     System.out.println(x+” “+z);     m1.methodA();     z=methodB(z+2)+x;     System.out.println(x+” “+z);     methodB(x,z);     System.out.println(x+” “+z);

}

int methodB(int y){     x=y+x;

System.out.println(x+” “+y);

return x+3;

}

void methodB(int z, int x){     z=z+1;     x=x+1;

System.out.println(z+” “+x);

}

}




class Maze{   static int x;

void methodA(){

int m;

x=5;

m=x+methodB(x);

System.out.println(x+” “+m);     m=methodB(m-3)+x;

System.out.println(x+” “+(m));     methodB(x,m);

System.out.println(x+” “+m+x);

}

int methodB(int y){

x=y*y;

System.out.println(x+” “+y);

return x+3;

}

void methodB(int z, int x){

z=z-2;     x=x*1;

System.out.println(z+” “+x);

}

}




<h1>Task 8</h1>

Create a class called Student as described below:

<ul>

 <li><strong>Fields: </strong>name, id, address, cgpa</li>

 <li><strong>Methods:</strong></li>

</ul>

public String getName() public void setName(String n) public String getID() public void setID(String i) public String getAddress() public void setAddress(String a) public double getCGPA()

public void setCGPA(double c)




Write a class called Main to write a main() method:

<ul>

 <li>public static void main(String[] args){</li>

</ul>

}

<ul>

 <li>Inside the main() method o Create 3 objects/instances of Student called john, mike and carol

  <ul>

   <li>Set their fields to some value using the public methods.</li>

   <li>Print the information of each Student using out.println()</li>

  </ul></li>

</ul>




<strong> </strong>

<h1>Task 9</h1>

Create a class called BankAccount as described below:

<ul>

 <li><strong>Fields: </strong>name, address, accountID, balance</li>

 <li><strong>Methods:</strong></li>

</ul>

public String getName() public void setName(String n) public String getAccountID() public void setAccountID(String i) public String getAddress() public void setAddress(String a) public double getBalance() public void setBalance(double c)

public void addInterest() //adds 7% of the balance




<ol>

 <li>Write a class called Main to write a main() method:

  <ul>

   <li>public static void main(String[] args){</li>

  </ul></li>

</ol>

}

<ul>

 <li>Inside the main() method o Create 3 objects/instances of BankAccount called acc1, acc2 and acc3</li>

</ul>

o Set their fields to some value using the public methods. o Call addInterest() on acc1 and acc3 o Print the information of each BankAccount using

System.out.println()




<ol start="2">

 <li>Add constructors to Student and BankAccount and use the constructor to set the field values.</li>

</ol>




<h2>Task 10</h2>




Design a class called <strong><sub>circle</sub></strong> which contains:

<ul>

 <li>Two <sub>private</sub> instance variables: <sub>radius</sub> (of the type <sub>double</sub>) and <sub>color</sub> (of the type String), with default value of <sub>0</sub> and “<sub>red</sub>“, respectively.</li>

 <li>Two <em>overloaded</em> constructors – a <em>default</em> constructor with no argument, and a constructor which takes a double argument for radius.</li>

 <li>Two <sub>public</sub> methods: <strong><sub>getRadius()</sub></strong> and <strong><sub>getArea()</sub>,</strong> which return the radius and area of this instance, respectively.</li>

</ul>







<h2>Task 11</h2>

Write a Java class Book with following features:

<ul>

 <li>Instance variables :

  <ul>

   <li><strong>title</strong> for the title of book of type String.</li>

   <li><strong>author</strong> for the author’s name of type String.</li>

   <li><strong>price </strong>for the book price of type double.</li>

  </ul></li>

 <li>Constructor:

  <ul>

   <li><strong>public Book (String title, String author, double price)</strong>: A constructor with parameters, it creates the Author object by setting the the fields to the passed values.</li>

  </ul></li>

 <li>Instance methods:

  <ul>

   <li><strong>public void setTitle(String title)</strong>: Used to set the title of book.</li>

   <li><strong>public void setAuthor(String author)</strong>: Used to set the name of author of book. o <strong>public void setPrice(double price)</strong>: Used to set the price of book. o <strong>public String getTitle()</strong>: This method returns the title of book. o <strong>public String getAuthor()</strong>: This method returns the author’s name of book.</li>

   <li><strong>public String toString()</strong>: This method printed out book’s details to the screen Write a separate class <strong>BookDemo</strong> with a main() method creates a Book titled “Developing Java Software” with authors Russel Winderand price 79.75. Prints the Book’s string representation to standard output (using System.out.println).</li>

  </ul></li>

</ul>




<h2>Task 12</h2>

Write a Java class Author with following features:

<ul>

 <li>Instance variables :

  <ul>

   <li><strong>firstName</strong> for the author’s first name of type String.</li>

   <li><strong>lastName</strong> for the author’s last name of type String.</li>

  </ul></li>

 <li>Constructor:

  <ul>

   <li><strong>public Author (String firstName, String lastName)</strong>: A constructor with parameters, it creates the Author object by setting the two fields to the passed values.</li>

  </ul></li>

 <li>Instance methods:

  <ul>

   <li><strong>public void setFirstName (String firstName)</strong>: Used to set the first name of author.</li>

   <li><strong>public void setLastName (String lastName)</strong>: Used to set the last name of author.</li>

   <li><strong>public String getFirstName()</strong>: This method returns the first name of the author. o <strong>public String getLastName()</strong>: This method returns the last name of the author.</li>

   <li><strong>public String toString()</strong>: This method printed out author’s name to the screen.</li>

  </ul></li>

</ul>

<strong> </strong>

<strong>   </strong>

<h2>Task 13</h2>

Write a Java class Clock for dealing with the day time represented by hours, minutes, and seconds. Your class must have the following features:

<ul>

 <li>Three instance variables for the hours (range 0 – 23), minutes (range 0 – 59), and seconds (range 0 – 59).</li>

 <li>Three constructors:

  <ul>

   <li>default (with no parameters passed; is should initialize the represented time to</li>

  </ul></li>

</ul>

12:0:0) o a constructor with three parameters: hours, minutes, and seconds. o a constructor with one parameter: the value of time in seconds since midnight (it should be converted into the time value in hours, minutes, and seconds)

<ul>

 <li>Instance methods:

  <ul>

   <li>a <em>set</em>-method method <strong>setClock() </strong>with one parameter <em>seconds</em> since midnight (to be converted into the time value in hours, minutes, and seconds as above).</li>

   <li><em>get</em>-methods <strong>getHours(), getMinutes(), getSeconds()</strong> with no parameters that return the corresponding values. o <em>set</em>-methods <strong>setHours(), setMinutes(), setSeconds()</strong> with one parameter each that set up the corresponding instance variables. o method <strong>tick()</strong> with no parameters that increments the time stored in a Clock object by one second. o method <strong>addClock()</strong> accepting an object of type Clock as a parameter. The method should add the time represented by the parameter object to the time represented in the current object. The new time should be returned as a clock object.</li>

   <li>Add an instance method <strong>toString()</strong> with no parameters to your class. toString() must return a String representation of the Clock object in the form “(hh:mm:ss)”, for example “(03:02:34)”. o Add an instance method <strong>tickDown()</strong> which decrements the time stored in a Clock object by one second.</li>

   <li>Add an instance method <strong>subtractClock()</strong> that takes one Clock parameter and returns the difference between the time represented in the current Clock object and the one represented by the Clock parameter. Difference of time should be returned as a clock object.</li>

  </ul></li>

</ul>

Write a separate class <strong>ClockDemo</strong> with a main() method. The program should:

<ul>

 <li>instantiate a Clock object firstClock using one integer <em>seconds</em> since midnight obtained from the keyboard.</li>

 <li>tick the clock ten times by applying its <em>tick()</em> method and print out the time after each tick.</li>

 <li>Extend your code by appending to it instructions instantiating a Clock object secondClock by using three integers (hours, minutes, seconds) read from the keyboard.</li>

 <li>Then tick the clock ten times, printing the time after each tick.</li>

 <li>Add the secondClock time in firstClock by calling method addClock.</li>

 <li>Print both clock objects calling toString method</li>

</ul>

Create a reference thirdClock that should reference to object of difference of firstClock and secondClock by calling the method subtractClock().




<h2>Task 14</h2>

Write a Java class Complex for dealing with complex number. Your class must have the following features:

<ul>

 <li>Instance variables :

  <ul>

   <li><strong>realPart</strong> for the real part of type double o <strong>imaginaryPart</strong> for imaginary part of type double.</li>

  </ul></li>

 <li>Constructor:

  <ul>

   <li><strong>public Complex ()</strong>: A default constructor, it should initialize the number to 0, 0) o <strong>public Complex (double realPart, double imaginaryPart)</strong>: A constructor with parameters, it creates the complex object by setting the two fields to the passed values.</li>

  </ul></li>

 <li>Instance methods:

  <ul>

   <li><strong>public Complex add (Complex otherNumber)</strong>: This method will find the sum of the current complex number and the passed complex number. The methods returns a new Complex number which is the sum of the two.  o <strong>public Complex subtract (Complex otherNumber)</strong>: This method will find the difference of the current complex number and the passed complex number.  The methods returns a new Complex number which is the difference of the two.</li>

   <li><strong>public Complex multiply (Complex otherNumber)</strong>: This method will find the product of the current complex number and the passed complex number. The methods returns a new Complex number which is the product of the two. o <strong>public Complex divide (Complex otherNumber)</strong>: This method will find the … of the current complex number and the passed complex number.  The methods returns a new Complex number which is the … of the two. o <strong>public void setRealPart (double realPart)</strong>: Used to set the real part of this complex number.</li>

   <li><strong>public void setImaginaryPart (double realPart)</strong>: Used to set the imaginary part of this complex number.</li>

   <li><strong>public double getRealPart()</strong>: This method returns the real part of the complex number</li>

   <li><strong>public double getImaginaryPart()</strong>: This method returns the imaginary part of the complex number</li>

   <li><strong>public String toString()</strong>: This method allows the complex number to be easily printed out to the screen</li>

  </ul></li>

</ul>

Write a separate class <strong>ComplexDemo</strong> with a main() method and test the Complex class methods.



















<strong><u>Task 15</u></strong>




Write a java class called <strong>BoroInt</strong> that uses a String value to store big integers and can carry out basic arithmetic operations on them.

<strong><em>Instance variable:</em></strong> String val

<strong><em>Overloaded constructors:</em></strong>

<ol>

 <li>default constructor: sets the value of val to “0”</li>

 <li>Takes a string value, checks whether it contains any non numerical values, if yes, then throws <strong>BoroIntErModdheNumberCharaArKisuDeyaJaiNaException </strong>(which is off course a custom exception which you must create &#x1f61b; ) … otherwise, copy the contents to val. <strong><em>Note: </em></strong>See method list below to see what you can use &#x1f61b;</li>

 <li>Takes an integer value, converts it to string and stores it in val.</li>

 <li>Takes a <strong>BoroInt</strong> object and copies the val of the parameter into it’s own val</li>

</ol>

<strong><em>Methods:</em></strong>

<strong>public String trim(String _val)</strong>

Removes all spaces in the String and returns a String value without any spaces.  <strong>public boolean validValue</strong>(<strong>String _val</strong>)

Returns true if the String _val doesn’t contain any non numerical characters and false otherwise.

<em> </em>

<strong>public BoroInt add(BoroInt _val) </strong>

Adds the value in the instance variable of the parameter to it’s own value and returns a new BoroInt object whose instance variable contains the result of the addition.

<strong>public BoroInt subtract(BoroInt _val)</strong>

Subtracts the value in the instance variable of the parameter from it’s own value and returns a new BoroInt object whose instance variable contains the result of the subtraction.

<strong>public BoroInt multiply(BoroInt _val)</strong>

Multiplies the value in the instance variable of the parameter with it’s own value and returns a new BoroInt object whose instance variable contains the result of the subtraction.

<strong>** public BoroInt divide(BoroInt _val) </strong>

Divides the value in it’s own instance variable by the value in the instance variable of the parameter and returns a new BoroInt object whose instance variable contains the result of the subtraction.

















