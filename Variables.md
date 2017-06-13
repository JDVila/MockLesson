<h1>Variables: Essentially Boxes that Hold Things.</h1>

As mentioned in a previous lesson (click <a href="https://docs.google.com/presentation/d/1gs1s35daJTko10G4WYKMvKptp0ZvZ7JUw2ZgdK1Gdqw/edit?usp=sharing">here</a> to view previous slideshow), A <b>program</b> is a set of instructions that tell a computer: <b>1)</b> What something is, <b>2)</b> To do something, <b>3)</b> How to do something, or <b>4)</b> Any combination of the three. A <b>programming language</b> is a way of writing instructions for computers, that people can also read and understand.

<b><i>Java is a type of programming language.</i></b><br>
<br>
Simply put, <b>Variables</b> are the simplest version of the "what something is" part!

Variables are essentially boxes that hold things for you.
<br>
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
There are four primitive data types for positive or negative whole numbers:<br>
<br>
&bull; byte<br>
&bull; short<br>
&bull; int<br>
&bull; long<br>
<br>
There are two primitive data types for positive or negative decimal numbers:<br>
<br>
&bull; float<br>
&bull; double<br>
<br>
There is one primitive data type for letters/punctuation/individual characters:<br>
<br>
&bull; char<br>
<br>
And one primitive data type for true or false values:<br>
<br>
&bull; boolean<br>
<h2>Variables for Whole Numbers</h2>
<br>
There are four primitive data types for whole numbers. They are different from each other based on <b><i>THE SIZE OF THE NUMBER</i></b> you can put in the box/variable.<br>
<br>
&bull; A <b>byte</b> type variable uses 1 byte (8 bits) of storage. It can be as small as -128, and as large as 127.<br>
<br>
&bull; A <b>short</b> type variable uses 2 bytes (16 bits) of storage. It can be as small as -32,768, and as large as 32,767.<br>
<br>
&bull; An <b>int</b> type variable uses 4 bytes (32 bits) of storage. It can be as small as -2,147,483,648, and as large as 2,147,483,647.<br>
<br>
&bull; A <b>long</b> type variable uses 8 bytes (64 bits) of storage. It can be as small as -9,223,372,036,854,775,808, and as large as 9,223,372,036,854,775,807.<br>
<br>
By the way that's 9 Quintillion, 223 Quadrillion, 372 Trillion, 36 Billion, 854 Million, 775 Thousand, 808. I had to actually Google how to say that correctly - that's how big of a number that is.<br>
<br>
If you want to know more about bits/bytes and storage, you can click <b>here</b>.<br>
<br>
🔑 Generally, programmers use the <b>int</b> type for storing whole numbers when using primitive types. This is because int variables are large enough to hold most numbers, and don't require as much storage as the <b>long</b> variable type.<br>
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
The number 42 is bigger than the minimum number an int variable can hold (-2,147,483,648), and smaller than the maximum number an int variable can hold (2,147,483,647), so that value assignment works! Good work!<br>
<br>
If you wanted to, you could even declare and assign an int variable at the same time! Here, try this:<br>
<br>
int intNumber = 42;<br>
<br>
When a <b>declared</b> int variable has been <b>assigned</b> a value, we say that the int variable has been <b>initialized</b>.<br>

<h2>Variables for Decimal Numbers</h2>
<br>
There are two primitive data types for decimal numbers. They are different from each other based on <b><i>THE LEVEL OF PRECISION</i></b> for the decimal number you want to put in the box/variable.<br>
<br>
<b>Let's think of it this way:</b> If you were to convert the fraction 1/4th into a decimal number, its value would be 0.25. The fraction 1/8th would convert to 0.125. We can see that as the fractions get smaller, the numbers after the decimal point increase in length. The numbers <b>AFTER</b> the decimal point are referred to as the <b>significand</b>, or the <b>mantissa</b>.<br>
<br>
&bull; A <b>float</b> type variable uses 4 bytes (32 bits) of storage, and it's significand/mantissa (numbers AFTER the decimal) is precise to around the 7th decimal place.<br>
<br>
&bull; A <b>double</b> type variable uses 8 bytes (64 bits) of storage, and it's significand/mantissa (numbers AFTER the decimal) is precise to around the 15th decimal place.<br>
<br>
🔑 Generally, programmers use the <b>double</b> type for storing decimal numbers when using primitive types. This is because even though float type variables take up less space, double variables are more precise - and the cost of losing precision might be higher than the space a smaller double variable might take up.<br>
<br>
You would <b>declare</b> a double variable like this:<br>
<br>
double dblNumber;<br>
<br>
When you declare a double variable, you are telling Java that this variable called dblNumber is now a new box that exists, and it can store a single thing, that is of type <b>double</b>.<br>
<br>
Let's <b>assign</b> a value to that variable. When you assign a value to a variable - just like in the example with an int variable, you are essentially putting something in the box you just created. In this case, the box is called dblNumber, and we can only put double values in it. Let's do that now:<br>
<br>
dblNumber = 0.125;<br>
<br>
Great! If you wanted to, just like with int variables, you could even declare and assign a double variable at the same time! Here, try this:<br>
<br>
double dblNumber = 0.125;<br>
<br>
When a <b>declared</b> double variable has been <b>assigned</b> a value, we say that the double variable has been <b>initialized</b>.<br>

<h2>Variables for Letters/Punctuation/Individual Characters</h2>
<br>
Java only has one primitive variable type for storing things like individual <b>unicode characters</b>. A <b>char</b> type variable uses 2 bytes (16 bits) of storage. It can be as small as 0, and as large as 65,536. It can never be a negative number.<br>
<br>
What is a unicode character, you might ask? Good question!<br>
<br>
A <b>unicode character</b> is a single letter/number/puctuation/keystroke/special character that takes up exactly one character space. For example:<br>
<br>
This is a character: <br><br><b>A</b><br>
<br>
This is also a character: <br><br><b>z</b><br>
<br>
This too is a character: <br><br><b>?</b><br>
<br>
And this: <br><br><b>%</b><br>
<br>
Also this: <br><br><b>$</b><br>
<br>
You might also be wondering why the value of a <b>char</b>, or character can be a number, as well as the character itself. This is because each unicode character has a corresponding <b>numerical value</b>.<br>
<br>
For example, you could declare and assign a char variable in several ways:<br>
<br>
<b>1)</b> char letterA = 'A';<br>
<br>
This is the easiest value assignment! Simply take the character, place it between two single quotes (single quotes look like this - ' ), and assign as usual! However, you could also use the unicode value, as seen below:<br>
<br>
<b>2)</b> char letterA = '\u0041';<br>
<br>
This is a great way to assign char values, since you might not have an understanding of the kinds of characters you wish to put in the variable (for example, foreign language characters like Chinese or Hindi). <b>Please remember to keep the unicode number inside the single quotes as well</b>. The third way uses the raw ASCII value:<br>
<br>
<b>3)</b> char letterA = 65;<br>
<br>
As you can see, it's just a number, and there is no need to place it between single quotes - but that number still matches the uppercase letter 'A' in value.<br>
<br>
Unicode values are written in <b>hexadecimal</b> numbers, or <b>hex</b> for short. ASCII values are written in <b>decimal</b> numbers, or <b>dec</b> for short. Look at the chart below for more information:<br>
<br>
<img src="https://naveenr.net/content/images/2017/03/ascii-codes.gif" alt="Unicode Chart" height="536" width="500">
🔑 <b>There is something very important to note here:</b> In Java, not all characters are the same. This means that uppercase 'A' is not the same as lowercase 'a' in numerical value. Look at the chart above - you will see that the uppercase letter 'A' has an ASCII or <b>dec</b> value of 65, while the lowercase letter 'a' has an ASCII or <b>dec</b> value of 97! Please remember this difference when assigning or comparing char values!<br>
<h2>Variables for True or False Values</h2>
<br>
Sometimes, it is important to keep track of things that are true or false. We can use the <b>boolean</b> primitive variable type to help us store that information. The boolean primitive type is named after the mathematician George Boole. George Boole did a lot of cool stuff. We will discuss absolutely none of that stuff today. If you want to know more, you can click and read the following link found <a href="https://en.wikipedia.org/wiki/George_Boole">here</a>.<br>
<br>
The process of declaring and assigning a boolean primitive variable is pretty straight-forward:<br>
<br>
boolean isThisRealLife = true;<br>
<br>
or:<br>
<br>
boolean doApplesTasteLikeMonkFish = false;<br>
<br>
As we can see, the variable is assigned with either a lowercase <b>true</b> or a lowercase <b>false</b>. However, boolean variables can also store the results of mathematical expressions. For example, if 2 plus 2 equals 4 (this would be true). However, before we explore how that works, we should first explore the difference between <b>assignment</b>, and <b>comparison</b>.<br>

<h2>Assigning vs. Comparing Values in Java</h2>
<br>
As we've done several times already - we can assign a value to a variable in three steps:<br>
<br>
<b>1) </b> state the type of the variable: <b>int</b><br>
<br>
<b>2) </b> declare the name of the variable: <b>intNumber</b><br>
<br>
<b>3) </b> assign the value of the variable: <b>42</b><br>
<br>
Which brings us the initialized variable:<br>
<br>
<b>int intNumber = 42;</b><br>
<br>
We also add a <b>semicolon</b>, or <b>;</b> character at the end of every statement, to let Java know that we are done with the statement.<br>
<br>
We can also assign a variable with a mathematical expression, like this:<br>
<br>
int nuNumber = 5 + 10;<br>
<br>
Java can only put one value into a primitive variable, so Java will perform the math for you, to make things work. 5 plus 10 is equal to 15, which means that the variable nuNumber is assigned the value of 15!<br>
<br>
But what if we wanted to see if certain values matched up? With the power of primitive variables combined, we can now do this! However, we will also need to use something called....<br>
<h3>Comparison Operators</h3><br>
<img src="http://introcs.cs.princeton.edu/java/11cheatsheet/images/comparison-ops.png" alt="Comparison Operators" height="254" width="500">
<br>
Remember how we mentioned ealier that boolean variables are boxes that contain either true or false values? Since mathematical expressions can also be true or false, we can store the result as a boolean as well! For example:<br>
<br>
<b>boolean thisIsTrue = 5 == 5;</b><br>
<br>
So, what value do you think is stored in the variable <b>thisIsTrue</b>, after the above expression? If you said <b>true</b>, you're right! Let's talk about the parts of that expression for a moment....<br>
<br>
&bull; <b>boolean</b> - we just defined the type of this variable as type boolean;<br>
<br>
&bull; <b>thisIsTrue</b> - this is the name of the variable;<br>
<br>
&bull; <b>= </b> - the "equals" sign that we use to assign value to the variable <b>thisIsTrue</b>;<br>
<br>
&bull; <b>5 == 5</b> - the "double-equals" comparison expression, where we check to see if 5 "is equal to" 5, which it is;<br><br>
&bull; <b>;</b> - and we close our statement with a ";" or semicolon.<br>
<br>
Let's look at another example:<br>
<br>
<b>boolean thisIsFalse = 5 >= 8;</b><br>
<br>
So, what value do you think is stored in the variable <b>thisIsFalse</b>, after the above expression? If you said <b>false</b>, you're right again! Let's examine this expression for a moment as well...<br>
<br>
&bull; <b>boolean</b> - we just defined the type of this variable as type boolean;<br>
<br>
&bull; <b>thisIsFalse</b> - this is the name of the variable;<br>
<br>
&bull; <b>= </b> - the "equals" sign that we use to assign value to the variable <b>thisIsFalse</b>;<br>
<br>
&bull; <b>5 >= 8</b> - the "greater-than-or-equal-to" comparison expression, where we check to see if 5 is "greater-than-or-equal-to" 8, which it is not;<br><br>
&bull; <b>;</b> - and we close our statement with a ";" or semicolon.<br>
<br>
🔑 <b>Major Key Alert:</b> Please remember the difference between the "=" or "equals" symbol, and the "==" or "double-equals" operator in Java. The single equals (=) is only for assigning values to variables or objects, while the double-equals (==) is used as a comparison operator, comparing two primitive values to each other.<br>
<h1>Strings - The "Sometimes Y" of Variable Types</h1>
Java, as mentioned before, has primitive types - but it also has something called object types. We will not go into objects today, because that's beyond the scope of today's lesson. However, because we use words and sentences all the time in Java, it's worth explaining our last value type today - Strings.<br>
<br>
A String is essentially a long collection of character primitives. Remember how we mentioned ealier that primitive variables can only hold one value? That's true, and since a string can hold more than one character, there is no way it can be a primitive. So, how would we save a string into a variable?<br>
<br>
Well, technically - we already did that in the beginning of the lesson. Let's look at the online form example from earlier:<br>
<br>
<b>String firstName = "Jose";</b><br>
<br>
Let's break it down part-by-part:<br>
<br>
&bull; <b>String</b> - we just defined the type of this variable as type <b>String</b> - unlike primitive types, the String type declaration begins with an uppercase "S", and not lowercase. This is because a String is of type <b>Object</b> - object types begin with an uppercase first letter;<br>
<br>
&bull; <b>firstName</b> - this is the name of the variable;<br>
<br>
&bull; <b>= </b> - the "equals" sign that we use to assign value to the variable <b>firstName</b>;<br>
<br>
&bull; <b>"Jose"</b> - we can see another difference, that the word <b>Jose</b> is wrapped in double-quotes. While char values are wrapped in single-quotes, String values are wrapped in double quotation marks;<br><br>
&bull; <b>;</b> - and we close our statement with a ";" or semicolon.<br>
<br>
<h1>Naming Conventions</h1>
Java likes it when you follow the rules. Java developers also like it when you follow the rules. Java will get angry at you if you use certain words as variable names. These words are called <b>Reserved Words</b>.
<h3>Reserved Words</h3>
Java will absolutely yell at you if you use any of the following words to name things in your code:<br>
<br>
<img src="https://raw.githubusercontent.com/JDVila/MockLesson/master/reserved_words.png" alt="Reserved Words in Java" height="344" width="500">
<h6>Don't be a hero - never use one of these "Reserved Words" as variable names.</h6>
<h3>Formatting A Variable Name</h3>
Just because Java likes your variable name, doesn't mean Java developers will like it. People will get on your case if you come up with weird names, unusual letter cases, or confusing number or character placement. Google has a whole website dedicated to how you should name your variables correctly in their style guide, but at this point, just consider these hard-and-fast rules for naming your variables:<br>
<br>
&bull; <b>Use camelCase</b>: camelCase is when you smush a couple of words together to form one word, but you keep the first word in all-lowercase, and capitalize the first letter of all the other words that come after (for example: firstName, lastName, thisIsTrue, thisIsFalse, etc.);<br>
<br>
&bull; <b>Don't Use Numbers as the First Character</b>: for example - <b>8ball</b> is considered incorrect, but <b>eight08sAndHeartBreak</b> works, despite the fact that it's also the name of a Kanye West album;<br>
<br>
&bull; <b>First Characters can be Letters, Underscores, or Dollar Signs</b>: You could use letterFirst, you could get away with <b>_titleColumn</b>, and even <b>$MoneyTalks</b> - but if you choose <b>kei$ha</b> as a variable, although you've done nothing syntatictally wrong, no one will actually want to be friends with you; and finally<br>
<br>
&bull; <b>No other Characters or Symbols. Sorry</b>: this one's pretty straight forward - as long as you follow the above rules, you should be okay for now. There are other rules for objects, constants, member variables, and other forms, but those are beyond what we are covering today.<br>
<br>
We did a lot. Here's a puppy:<br>
<br>
<img src="http://www.localpuppybreeders.com/wp-content/uploads/2014/11/Happy-Puppy.jpg" alt="Reserved Words in Java" height="280" width="240">
