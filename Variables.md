<h1>Variables: Essentially Boxes that Hold Things.</h1>

As mentioned in a previous lesson (click <a href="https://docs.google.com/presentation/d/1gs1s35daJTko10G4WYKMvKptp0ZvZ7JUw2ZgdK1Gdqw/edit?usp=sharing">here</a> to view previous slideshow), A <b>program</b> is a set of instructions that tell a computer: <b>1)</b> What something is, <b>2)</b> To do something, <b>3)</b> How to do something, or <b>4)</b> Any combination of the three. A <b>programming language</b> is a way of writing instructions for computers, that people can also read and understand.

<b><i>Java is a type of programming language.</i></b><br>
<br>
Simply put, <b>Variables</b> are the simplest version of "what something is" part!

Variables are essentially boxes that hold things for you.

<img src="http://hackathon-in-a-box.org/img/box.png" alt="Submit Button" height="250" width="250"><br>
<h6>This box is a visual representation of a variable. Semiotics!</h6><br>
<br>
For example, let's say you are filling out an online form:<br><br>

<b>&emsp;First Name: ______________ </b>

<b>&emsp;Last Name: ______________ </b>

<b>&emsp;&emsp;&emsp;&emsp;Age: ______________ </b>
<br>
<img src="https://raw.githubusercontent.com/JDVila/MockLesson/master/send_button.png" alt="Submit Button" height="55" width="250">
<br><br>
The answers to each of those questions would need to be stored in three separate "boxes". A "box" for a "First Name," a box for a "Last Name," and a "box" for the number "Age."<br>
<br>
First Name = Jose<br>
Last Name = Vila<br>
Age = 36<br>
<br>
Easy enough, yes? However, Java is something called a <b>Strongly-Typed</b> language. This means that if you are going to put something in a box (or variable), you have to match the kind of box with the types of things that go into those boxes. In Java, there are simple boxes just for whole numbers of different sizes, shorter or longer decimal numbers, individual letters/characters, and whether something is true, or untrue (false).<br>
<br>
String firstName = "Jose";<br>
String lastName = "Vila";<br>
int age = 36;

<h2>Primitive Variables</h2>
Java has eight "primitive," or non-object data types. All primitive means is that they are the most basic data types that Java allows you to work with. It is the actual value, and not a reference to the value (we'll learn more about the difference between those two in a later lesson).<br>
<br>
There are four for positive or negative whole numbers:<br>
<br>
&bull; byte<br>
&bull; short<br>
&bull; int<br>
&bull; long<br>
<br>
There are two for positive or negative decimal numbers:<br>
<br>
&bull; float<br>
&bull; double<br>
<br>
There is one for letters/punctuation/individual characters:<br>
<br>
&bull; char<br>
<br>
And one for true or false values:<br>
<br>
&bull; boolean<br>
<h2>Variables for Whole Numbers</h2>
<br>
There are four primitive data types for whole numbers. They are different from each other based on <b><i>THE SIZE OF THE NUMBER</i></b> you want to put in the box/variable.<br>
<br>
&bull; A <b>byte</b> type variable uses 1 byte (8 bits) of storage. It can be as small as -128, and as large as 127.<br>
<br>
&bull; A <b>short</b> type variable uses 2 bytes (16 bits) of storage. It can be as small as -32,768, and as large as 32,767.<br>
<br>
&bull; An <b>int</b> type variable uses 4 bytes (32 bits) of storage. It can be as small as -2,147,483,648, and as large as 2,147,483,647.<br>
<br>
&bull; A <b>long</b> type variable uses 8 bytes (64 bits) of storage. It can be as small as -9,223,372,036,854,775,808, and as large as 9,223,372,036,854,775,807.<br>
<br>
If you want to know more about bits/bytes and storage, you can click <b>here</b>.<br>
<br>
🔑 Generally, programmers use the <b>int</b> type for storing numbers when using primitive types. This is because int variables are large enough to hold most numbers, and don't require as much storage as the <b>long</b> variable type.<br>
<br>
You would <b>declare</b> an int variable like this:<br>
<br>
int intNumber;<br>
<br>
When you declare an int variable, you are telling Java that this variable called intNumber is now a new box that exists, and it can store a single thing, that is of type <b>int</b>.<br>
<br>
Let's <b>assign</b> a value to that variable. When you assign a value to a variable, you are essentially putting something in the box you just created. In this case, the box is called intNumber, and we can only put int values in it. Let's do that now:<br>
<br>
intNumber = 42;<br>
<br>
If you wanted to, you could even declare and assign a variable at the same time! Here, try this:<br>
<br>
int intNumber = 42;<br>

<h2>Variables for Decimal Numbers</h2>
<br>
There are two primitive data types for decimal numbers. They are different from each other based on <b><i>THE LEVEL OF PRECISION</i></b> for the decimal number you want to put in the box/variable.<br>
<br>
<b>Let's think of it this way:</b> If you were to convert the fraction 1/4th into a decimal number, its value would be 0.25. The fraction 1/8th would convert to 0.125. We can see that as the fractions get smaller, the numbers after the decimal point increase in length. The numbers after the decimal point are referred to as the <b>significand</b>, or the <b>mantissa</b>.<br>
<br>
&bull; A <b>float</b> type variable uses 4 bytes (32 bits) of storage, and it's significand/mantissa (numbers AFTER the decimal) is precise to around the 7th decimal place.<br>
<br>
&bull; A <b>double</b> type variable uses 8 bytes (64 bits) of storage, and it's significand/mantissa (numbers AFTER the decimal) is precise to around the 15th decimal place.<br>
<br>
🔑 Generally, programmers use the <b>double</b> type for storing decimal numbers when using primitive types. This is because even though float type variables take up less space, double variables are more precise - and the cost of losing precision might be higher than the space a smalller double variable might take up.<br>

<h2>Variables for Letters/Punctuation/Individual Characters</h2>
<br>
Java only has one primitive variable type for storing things like individual letters
