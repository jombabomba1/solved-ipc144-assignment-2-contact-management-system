Download Link: https://assignmentchef.com/product/solved-ipc144-assignment-2-contact-management-system
<br>
Assignment 2 uses assignment 1 and focuses on a “Contact Management System”.  This assignment continues to emphasize modularization by compartmentalizing highly cohesive and tightly coupled tasks into modules (*.h and *.c files).  This strategy will reduce redundant coding throughout all parts of the application.

<h1>Deadlines</h1>

This assignment is broken into four (4) parts:

<h2>Milestone 1</h2>

Download or clone Assignment 2 (<strong>A2</strong>) from <a href="https://github.com/Seneca-144100/IPC-Project">https://github.com/Seneca-144100/IPC-Project</a>

Open the project file <strong>A2MS1</strong> and look inside (expand “Header Files” and “Source Files” folders – see figure 2.1.1).  You will find two modules:




<table width="414">

 <tbody>

  <tr>

   <td width="132"><strong>Module </strong></td>

   <td width="126"><strong>Header File </strong></td>

   <td width="156"><strong>Source File </strong></td>

  </tr>

  <tr>

   <td width="132">Contacts</td>

   <td width="126">contacts.h</td>

   <td width="156">contacts.c</td>

  </tr>

  <tr>

   <td width="132">Contact Helpers</td>

   <td width="126">contactHelpers.h</td>

   <td width="156">contactHelpers.c</td>

  </tr>

 </tbody>

</table>




<u>Figure</u>: 2.1.1 – Visual Studio Project Contents

<strong><u>Contacts Header File</u></strong><strong> (.h)</strong>

<h3>Structures</h3>

Open the <strong>contacts.h</strong> file and copy the structures (Name, Address, Numbers, and Contact) from the file <strong>contacts.h</strong> in <em>Assignment 1</em>.  Be careful not to paste over the helpful comments in the provided <strong>contacts.h</strong> file!




<h3>Function Prototypes</h3>

<ol>

 <li>Copy the function prototypes (<strong>getName</strong>, <strong>getAddress</strong>, and <strong>getNumbers</strong>) from the file <strong>h</strong> in <em>Assignment 1 (Milestone 4)</em>. Again, be careful not to paste over the helpful comments in the provided <strong>contacts.h</strong> file!</li>

</ol>




<ol start="2">

 <li>Declare an additional function prototype:</li>

</ol>

<h4>void getContact(struct Contact *contact);</h4>

<ul>

 <li>This function has one parameter that receives a pointer to a Contact.</li>

 <li>The details on how this function should work is described in Milestone 2.</li>

</ul>




<strong><u>Contacts Source File</u></strong><strong> (.c)</strong>

Open the <strong>contacts.c</strong> source code file.

<h3>Libraries</h3>

In order to define the functions that were declared as prototypes in the <strong>contacts.h</strong> file, this source file needs visibility of their existence.  This is accomplished by including the required header library file. Include the <strong>contacts.h</strong> header file (see source code comments).

<h3> Function Definitions</h3>

<ol>

 <li>Copy the function definitions (<strong>getName</strong>, <strong>getAddress</strong>, and <strong>getNumbers</strong>) from the file <strong>c</strong> in <em>Assignment 1 (Milestone 4)</em>.</li>

</ol>




<ol start="2">

 <li>Add an <strong>empty</strong> definition for the new function <strong>getContact</strong> (see the prototype declared in the <strong>h</strong> file) – refer to the source comments for placement. For this milestone you don’t have to define the details for this function (this will be done in Milestone 2) so for now, specify an empty code block:</li>

</ol>

<strong>getContact function header goes here… </strong>

{

// Use an open and close curly brace with a blank line }

<h4><u>Contact Helper Header File</u> (.h)</h4>

The contact helper module contains a group of common functions for use in other source code modules in the application.  Other modules will be able to access these functions (without having to recode them) by including this header file.

<h3>Function Prototypes</h3>

Open the <strong>contactHelpers.h</strong> file.  To help you get started, you will notice the prototype for the clearKeyboard function is already done for you.

<h4>void clearKeyboard(void);</h4>

<ul>

 <li><strong>clearKeyboard</strong> does not return a value and has no parameters.</li>

 <li>The details on how this function should work is described in Milestone 2.</li>

</ul>

Add the following additional helper function prototypes:

<strong>void </strong><strong>pause</strong><strong>(void)</strong><strong>;</strong>

<ul>

 <li><strong>pause </strong>does not return a value and has no parameters.</li>

 <li>The details on how this function should work is described in Milestone 2.</li>

</ul>

<h4>int getInt(void);</h4>

<ul>

 <li><strong>getInt </strong>returns an integer value and has no parameters.</li>

 <li>The details on how this function should work is described in Milestone 2.</li>

</ul>

<h4>int getIntInRange(int min, int max);</h4>

<ul>

 <li><strong>getIntInRange </strong>returns an integer value and receives two (2) integer parameters.</li>

 <li>The details on how this function should work is described in Milestone 2.</li>

</ul>

<h4>int yes(void);</h4>

<ul>

 <li><strong>yes </strong>returns an integer value and has no parameters.</li>

 <li>The details on how this function should work is described in Milestone 2.</li>

</ul>

<h4>int menu(void);</h4>

<ul>

 <li><strong>menu </strong>returns an integer value and has no parameters.</li>

 <li>The details on how this function should work is described in Milestone 2.</li>

</ul>

<h4>void contactManagerSystem(void);</h4>

<ul>

 <li><strong>contactManagerSystem </strong>does not return a value and has no parameters.</li>

 <li>The details on how this function should work is described in Milestone 2.</li>

</ul>




<strong><u>Contact Helper Source File</u></strong><strong> (.c)</strong>

Open the <strong>contactHelpers.c</strong> source code file.

<h3>Libraries</h3>

Just as the <strong>contacts.c</strong> source code file included the <strong>contacts.h</strong> header file, the <strong>contactHelpers.c</strong> source code file should include the <strong>contactHelpers.h</strong> header file. Including the header file exposes the prototyped functions before they are defined (see source code comments).

<h3>Function Definitions</h3>

Add an empty definition for each function prototyped in the <strong>contactHelpers.h</strong>.  You will notice the clearKeyboard function has been done for you.  Follow this example for the remaining functions (refer to the source code comments for placement).




For this milestone, you don’t have to define the details for the functions (the details are described in Milestone 2).




<strong>Milestone 1 Submission </strong>

Milestone 1 is to be done in the lab and shown to your instructor, there is no need to submit on matrix.

<h2>Milestone 2</h2>

Open the project file <strong>A2MS2</strong> and look inside (expand “Header Files” and “Source Files” folders – see figure 2.2.1).  You will notice an additional source code file <strong>a2ms2.c</strong> (do not modify this file).  This is the main file used to assess your functions to determine if they work to this milestone’s specifications.

<u>Figure</u>: 2.2.1 – Visual Studio Project Contents

<h3><u>Header Files</u></h3>

<strong>contact.h and contactHelpers.h</strong>

There are no changes required to these files for this milestone.  Consult the comments provided in the header files (.h) for these modules and copy the appropriate contents from Milestone 1.

<h3><u>Contact Helper Source File</u> (.c)</h3>

<ol>

 <li>Open the <strong>c</strong> source code file.</li>

</ol>

<strong>Reminder</strong>:  Be sure to include the contactHelpers.h header file!

To help you get started, notice that the clearKeyboard function is done for you.

<ol start="2">

 <li>For the remaining functions, copy the empty functions from the <strong>c</strong> file in <em>Milestone 1</em> (consult the source code comments for placement – be careful not to replace the clearKeyboard function that is already provided for you).</li>

</ol>




<ol start="3">

 <li>Complete the full function definition for each function using the descriptions below:</li>

</ol>

<h4>void clearKeyboard(void);</h4>

<ul>

 <li><strong>clearKeyboard</strong> does not return a value and has no parameters.</li>

 <li>This function makes sure the keyboard input buffer is clear of any residual character by reading from the input buffer character by character until it reads a new line character.</li>

 <li>This function is provided for you – please consult the IPC144 course notes in the section “Input Functions” to learn about the standard input output library (stdio) getchar() function.</li>

</ul>

<strong>void </strong><strong>pause</strong><strong>(void)</strong><strong>;</strong>

<ul>

 <li><strong>pause </strong>does not return a value and has no parameters.</li>

 <li>This function pauses the execution of the application by displaying a message and waiting for the user to press the &lt;ENTER&gt; key.</li>

 <li>Display the following line and DO NOT include a newline character:</li>

</ul>

&gt;(Press Enter to continue)&lt;

<ul>

 <li>After displaying the above message, call the clearKeyboard</li>

</ul>




<strong>Note</strong>: The clearKeyboard function is used for a foolproof &lt;ENTER&gt; key entry

<strong>       </strong> getInt(void);

<ul>

 <li><strong>getInt </strong>returns an integer value and has no parameters.</li>

 <li>This function gets a valid integer from the keyboard and returns it. If the value entered is not a valid integer an error message should be displayed:</li>

</ul>

&gt;*** INVALID INTEGER *** &lt;Please enter an integer&gt;: &lt;

<ul>

 <li>This function should continue to prompt the user for a valid integer.</li>

 <li>This function must be foolproof and guarantee an integer value is entered and returned.</li>

</ul>

<strong><u>Hint</u></strong>

You can use scanf to read an integer and a character (“%d%c”) in one call and then assess if the second value is a newline character.  If the second character is a newline (the result of an &lt;ENTER&gt; key press), scanf read the first value successfully as an integer.

If the second value (character) is not a newline, the value entered was not an integer or included additional non-integer characters.  If any invalid entry occurs, your function should call the clearKeyboard function, followed by displaying the error message described above and continue to prompt for a valid integer. Review the following flowchart that describes this process:

<h4> getIntInRange(int min, int max);</h4>

<ul>

 <li><strong>getIntInRange </strong>returns an integer value and receives two (2) integer parameters.</li>

 <li>This function uses getInt to receive a valid integer and returns it only if the value entered is within the lower-bound (first parameter) and upper-bound (second parameter) range (<strong>inclusive</strong>).</li>

 <li>If the integer entered is not within the valid range, the following error message should be displayed:</li>

</ul>

&gt;*** OUT OF RANGE *** &lt;Enter a number between [param-1] and [param-2]&gt;: &lt;

<strong>Note</strong>:  <em>Substitute the “[param-1]” and “[param-2]” with the function parameter values</em>




<ul>

 <li>This function should be a foolproof call to ensure an integer is entered within a given range. Therefore, it should continue to prompt the user for an entry until a valid integer is within the specified range.</li>

</ul>

<h4>int yes(void);</h4>

<ul>

 <li><strong>yes </strong>returns an integer value and has no parameters.</li>

 <li>This function prompts the user for a <strong>single character</strong> entry</li>

 <li>The character entered is only valid if it is a “Y”, “y”, “N”, or “n”. Any other value entered (including more than one character) is an error and should display the following message:</li>

</ul>

&gt;*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: &lt;

<strong><u>Hint</u></strong>

This function is very similar to the getInt function only this function looks for a character as the first value.  If the second value is not a newline character it is definitely an error as it won’t be a single character entry (be sure to call the clearKeyboard function to clear the input buffer).  If the second value is a newline character, then assess if the first value is one of the four (4) valid characters.  If it isn’t one of the valid four (4) characters, then it is an error.




<ul>

 <li>This function should continue to prompt the user for an entry until one of the four (4) valid characters is entered.</li>

 <li>When a valid value is entered, the function should return an integer value of 1 when the value is “Y” or “y”. Otherwise it should return 0.</li>

</ul>




<strong>       </strong>

<h4> menu(void);</h4>

<ul>

 <li><strong>menu </strong>returns an integer value and has no parameters.</li>

 <li>This function should display the following menu:</li>

</ul>

&gt;Contact Management System&lt;

&gt;————————-&lt;  (there are 25 dashes)

&gt;1. Display contacts&lt;

&gt;2. Add a contact&lt;

&gt;3. Update a contact&lt;

&gt;4. Delete a contact&lt;

&gt;5. Search contacts by cell phone number&lt;

&gt;6. Sort contacts by cell phone number&lt;

&gt;0. Exit&lt;

&gt;&lt;

&gt;Select an option:&gt; &lt;

<ul>

 <li>Prompt for user entry an integer value between the values 0-6 inclusive</li>

 <li>Any other value entered or an integer that is not within the 0-6 range is an error</li>

 <li>The function should continue to prompt for an integer value within the 0-6 range until a valid value is entered.</li>

 <li>When a valid integer value is entered, this value is returned.</li>

</ul>




<strong><u>Hint</u></strong>

This logic sounds familiar… perhaps there is already a function that can help you get an integer value within a specified range…




<h4>void contactManagerSystem(void);</h4>

<ul>

 <li><strong>contactManagerSystem </strong>does not return a value and has no parameters.</li>

 <li>This function is the heart of the application and will run the whole program.</li>

 <li>This function starts by showing the menu for the system and receives the user’s selection</li>

 <li>If the user enters 1, it displays:</li>

</ul>

<strong>&gt;</strong>&lt;&lt;&lt; Feature 1 is unavailable &gt;&gt;&gt;<strong>&lt;</strong><strong><em>  </em></strong><em>(followed by two (2) newlines) </em>If the user enters 2, it displays:

<strong>&gt;</strong>&lt;&lt;&lt; Feature 2 is unavailable &gt;&gt;&gt;<strong>&lt;</strong><strong><em>  </em></strong><em>(followed by two (2) newlines) </em>If the user enters 3, it displays:

<strong>&gt;</strong>&lt;&lt;&lt; Feature 3 is unavailable &gt;&gt;&gt;<strong>&lt;</strong><strong><em>  </em></strong><em>(followed by two (2) newlines) </em>If the user enters 4, it displays:

<strong>&gt;</strong>&lt;&lt;&lt; Feature 4 is unavailable &gt;&gt;&gt;<strong>&lt;</strong><strong><em>  </em></strong><em>(followed by two (2) newlines) </em>If the user enters 5, it displays:

<strong>&gt;</strong>&lt;&lt;&lt; Feature 5 is unavailable &gt;&gt;&gt;<strong>&lt;</strong><strong><em>  </em></strong><em>(followed by two (2) newlines) </em>If the user enters 6, it displays:

<strong>&gt;</strong>&lt;&lt;&lt; Feature 6 is unavailable &gt;&gt;&gt;<strong>&lt;</strong><strong><em>  </em></strong><em>(followed by two (2) newlines) </em>

For selections between 1 and 6, the application should <strong>pause</strong> and then return to displaying the menu.

<ul>

 <li>If the user enters 0, prompt to exit the application. Display the following:</li>

</ul>

<strong>&gt;</strong>Exit the program? (Y)es/(N)o: <strong>&lt;  </strong>




Wait for the user to enter “Y”, ”y”, “N” or “n” (for Yes or No).

If the user replies Yes (“Y”,”y”), it will end the program displaying the following message:




<strong>&gt;</strong>Contact Management System: terminated<strong>&lt; </strong><em>(followed by a newline)</em>




Otherwise, if the user entered No (“N”,”n”), the application continues to display the menu.

<ul>

 <li>The following is a general pseudo code for a menu driven user interface. Using this pseudo code is optional. You can use any other logic if you like.</li>

</ul>

Menu driver pseudo code: while it is not done    display menu

get selected option from user    check selection:

option one selected          act accordingly       end option one       option two selected          act accordingly       end option two

.

.

Exit is selected          program is done       end exit    end check end while




<h3><u>Contacts Source File</u> (.c)</h3>

Open the <strong>contacts.c</strong> source code file.

<ol>

 <li>Open the <strong>c</strong> source code file.</li>

</ol>

<strong>Reminder</strong>:  Be sure to include the <strong>contacts.h</strong> header file!

The contact helpers module contains additional functions that can be used to streamline some functions previously coded for getting the Name, Address, and Numbers parts of a Contact.  To make these helper functions available for use in this source file include the <strong>contactHelpers.h</strong> header file (see the source code comments for placement).

<ol start="2">

 <li>Copy the functions from the <strong>c</strong> file in <em>Milestone 1</em> (see the source code comments for placement – be careful not to replace any additional helpful comments)</li>

</ol>




<ol start="3">

 <li>Update the functions getName, getAddress, and getNumbers to use any of the new functions created in the contactHelpers.h library (wherever applicable). See source code comments for some suggestions.</li>

</ol>




<ol start="4">

 <li>Update function getNumbers so that the cell phone number entry is <strong>mandatory</strong> (don’t ask if the user wants to enter this value)</li>

</ol>




<ol start="5">

 <li>Define the new function prototyped in <em>Milestone 1</em> getContact using the following description:</li>

</ol>

<h4>void getContact(struct Contact *contact);</h4>

<ul>

 <li>This function does not return a value but has one parameter that receives a pointer to a Contact.</li>

 <li>The purpose of this function is to set the values for a Contact using the pointer parameter variable (set the Contact it points to).</li>

 <li>Use the pointer parameter received to this function to supply the appropriate Contact member to the “get” functions (getName, getAddress, and getNumbers) to set the values for the Contact.</li>

</ul>

<strong> </strong>

<strong> </strong>

<h1>Sample Output</h1>

Below is a sample output.  User input values are identified in <strong>BOLD</strong>.  Your output should match exactly:

—————————————— Testing: Yes()

——————————————

Please enter ‘Y’ &gt; <strong>Y</strong>     Result: 1

Please enter ‘y’ &gt; <strong>y</strong>     Result: 1

Please enter ‘N’ &gt; <strong>N</strong>

Result: 0

Please enter ‘yes’, then ‘no’, then ‘n’ &gt; <strong>yes</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>no</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>n</strong>

Result: 0




——————————————

Testing: pause()

——————————————

(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




—————————————— Testing: getInt()

—————————————— Enter ‘ipc’, then ‘144’ &gt; <strong>ipc</strong>

*** INVALID INTEGER *** &lt;Please enter an integer&gt;: <strong>144</strong>

Integer entered: 144




—————————————— Testing: getIntInRange(int,int)

——————————————

Enter ‘seneca’, then ’99’, then ‘501’, then ‘250’ &gt; <strong>seneca</strong> *** INVALID INTEGER *** &lt;Please enter an integer&gt;: <strong>99</strong>

<table width="22">

 <tbody>

  <tr>

   <td width="22"><strong>501</strong></td>

  </tr>

  <tr>

   <td width="22"><strong>250</strong></td>

  </tr>

 </tbody>

</table>

*** OUT OF RANGE *** &lt;Enter a number between 100 and 500&gt;:

*** OUT OF RANGE *** &lt;Enter a number between 100 and 500&gt;:

Integer entered: 250




Enter ‘100’ &gt; <strong>100</strong>

Integer entered: 100 Enter ‘500’ &gt; <strong>500</strong>

Integer entered: 500




—————————————— Testing: getContact(struct Contact *)

——————————————

Please enter the contact’s first name: <strong>Tom See John </strong>

Do you want to enter a middle initial(s)? (y or n): <strong>yes</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>y</strong>

Please enter the contact’s middle initial(s): <strong>How Wong R. U.</strong>

Please enter the contact’s last name: <strong>Song Sing</strong>

Please enter the contact’s street number: <strong>one two</strong>

*** INVALID INTEGER *** &lt;Please enter an integer&gt;: <strong>-99</strong>

*** INVALID STREET NUMBER *** &lt;must be a positive number&gt;: <strong>99</strong>

Please enter the contact’s street name: <strong>Keele Street</strong>

Do you want to enter an apartment number? (y or n): <strong>y</strong>

Please enter the contact’s apartment number: <strong>-1920</strong>

*** INVALID APARTMENT NUMBER *** &lt;must be a positive number&gt;: <strong>1920</strong>

Please enter the contact’s postal code: <strong>A8A 3J3 R1W</strong>

Please enter the contact’s city: <strong>North Bay</strong>

Please enter the contact’s cell phone number: <strong>9051116666</strong>

Do you want to enter a home phone number? (y or n): <strong>n y</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>n</strong>

Do you want to enter a business phone number? (y or n): <strong>n</strong>




Values Entered:

Name: Tom See John How Wo Song Sing Address: 99|Keele Street|1920|A8A 3J3|North Bay

Numbers: 9051116666||




——————————————

Testing: contactManagerSystem()

——————————————

Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>9</strong>

*** OUT OF RANGE *** &lt;Enter a number between 0 and 6&gt;: <strong>1</strong>




&lt;&lt;&lt; Feature 1 is unavailable &gt;&gt;&gt;




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>4</strong>




&lt;&lt;&lt; Feature 4 is unavailable &gt;&gt;&gt;




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>6</strong>




&lt;&lt;&lt; Feature 6 is unavailable &gt;&gt;&gt;




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>0</strong>




Exit the program? (Y)es/(N)o: <strong>n</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>0</strong>




Exit the program? (Y)es/(N)o: <strong>y</strong>




Contact Management System: terminated




—————————————— Testing: Assign#2 – MS #2 test completed

——————————————

<h2>Milestone 2 Reflection</h2>

Please provide answers to the following in a text file named <strong>reflect.txt.</strong>

In <u>three</u> or more paragraphs and a <strong><u>minimum</u> of 150 words</strong>, explain what you learned while doing these first two milestones.  In <strong><u>addition to what you learned</u></strong>, <strong>y</strong><strong>our reflection should <u>also include the</u> <u>following</u></strong>:

<ul>

 <li>An explanation of the term “function” and briefly discuss the need for functions in any language.</li>

 <li>An explanation why you think the “helper” functions are in a different module and why those functions were not included in the “contacts” module.</li>

</ul>

<strong>Reflections will be graded based on the published rubric (</strong><a href="https://github.com/Seneca-144100/IPC-Project/tree/master/Reflection%20Rubric.pdf">https://github.com/Seneca</a><a href="https://github.com/Seneca-144100/IPC-Project/tree/master/Reflection%20Rubric.pdf">144100/IPC-Project/tree/master/Reflection%20Rubric.pdf</a><a href="https://github.com/Seneca-144100/IPC-Project/tree/master/Reflection%20Rubric.pdf"><strong>)</strong></a><strong>.</strong>

<strong><u>Example</u></strong><strong>:  </strong>

<strong>An example reflection answer for <u>Workshop #2</u> is available demonstrating the minimum criteria: </strong><a href="https://github.com/Seneca-144100/IPC-Project/tree/master/Example%20Reflection-WS_2.pdf"><strong>https://github.com/Seneca-144100/IPC-Project/tree/master/Example%20Reflection-WS_2.pdf</strong></a>




<h2>Milestone 2 Submission</h2>

If not on matrix already, upload your <strong>contacts.h</strong>,<strong> contacts.c</strong><strong>,</strong><strong> contactHelpers.h</strong><strong>,</strong><strong> contactHelpers.c</strong><strong>,</strong><strong> a2ms2.c</strong>, and <strong>reflect.txt</strong> files to your matrix account. Compile your code as follows:

<h3>&gt; gcc -Wall -o ms2 contacts.c contactHelpers.c a2ms2.c &lt;ENTER&gt;</h3>

This command will compile your code and name your executable “<strong>ms2</strong>”.  Execute <strong>ms2</strong> and make sure everything works properly.

Then run the following script from your account and follow the instructions (replace profname.proflastname with your professors Seneca userid and <u>replace</u> <strong>NAA</strong> with <u>your</u> section):

<strong>~profname.proflastname/submit 144a2ms2/NAA_ms2 &lt;ENTER&gt;</strong><strong>  </strong>

<h1><u>Please Note</u></h1>

<ul>

 <li>A successful submission does not guarantee full credit for this workshop.</li>

 <li>If the professor is not satisfied with your implementation, your professor may ask you to resubmit. Resubmissions will attract a penalty.</li>

</ul>

<h2>Milestone 3</h2>

<strong> </strong>

Download or clone Assignment 2 (<strong>A2</strong>) from <a href="https://github.com/Seneca-144100/IPC-Project">https://github.com/Seneca-144100/IPC-Project</a>

Open the project file <strong>A2MS3</strong> and look inside (expand “Header Files” and “Source Files” folders).

This milestone introduces the remaining function prototypes required to complete the contacts management system.  You have three tasks to perform for this milestone:

<ol>

 <li>Declare new function prototypes in <strong>h</strong></li>

 <li>Define the new functions with empty code blocks in <strong>c</strong></li>

 <li>Update <strong>h</strong> with safeguard and <strong>contact.c</strong> to use new function getTenDigitPhone</li>

</ol>

<h3><u>Contact Helper Header File</u> (.h)</h3>

Open the <strong>contactHelpers.h</strong> file.  Refer to the comments in the file and copy/paste your code from MS2 where directed.

You will need to include the <strong>contacts.h</strong> header file so the new functions (parameters) will be able to use the structures defined in that module (see source comments for placement).

<h3>Function Prototypes</h3>

You will notice there are two (2) prototypes already prepared:

<h4>void getTenDigitPhone(char phoneNum[]);</h4>

<ul>

 <li><strong>getTenDigitPhone</strong> does not return a value and expects a character array sized for 10 characters plus the null terminator.</li>

 <li>The next section describing the <strong>c</strong> source file explains this function and its use.</li>

</ul>

<strong>int</strong><strong> findContactIndex(</strong><strong>const</strong> <strong>struct</strong> <strong>Contact </strong><strong>contacts[], </strong><strong>int </strong><strong>size,                                                 </strong><strong>const</strong> <strong>char </strong><strong>cellNum[]); </strong>

<ul>

 <li><strong>findContactIndex</strong> returns an integer and expects a <strong>Contact</strong> array (marked constant so changes can’t be made to it), an integer, and a character array.</li>

 <li>The details on how this function should work is described in Milestone 4.</li>

</ul>

Add the following additional function prototypes:

<h4>void displayContactHeader(void);</h4>

<ul>

 <li><strong>displayContactHeader </strong>does not return a value and has no parameters.</li>

 <li>The details on how this function should work is described in Milestone 4.</li>

</ul>

<h4>void displayContactFooter(int count);</h4>

<ul>

 <li><strong>displayContactFooter</strong> does not return a value and receives one integer parameter.</li>

 <li>The details on how this function should work is described in Milestone 4.</li>

</ul>

<h4>void displayContact(const struct Contact *contact);</h4>

<ul>

 <li><strong>displayContact</strong> does not return a value and receives a constant <strong>Contact</strong> pointer (cannot be updated) parameter.</li>

 <li>The details on how this function should work is described in Milestone 4.</li>

</ul>

<h4>void displayContacts(const struct Contact contacts[], int size);</h4>

<ul>

 <li><strong>displayContacts</strong> does not return a value and receives a constant <strong>Contact</strong> array (cannot be updated), and an integer for parameters.</li>

 <li>The details on how this function should work is described in Milestone 4.</li>

</ul>

<h4>void searchContacts(const struct Contact contacts[], int size);</h4>

<ul>

 <li><strong>searchContacts</strong> does not return a value and receives a constant <strong>Contact</strong> array (cannot be updated), and an integer for parameters.</li>

 <li>The details on how this function should work is described in Milestone 4.</li>

</ul>

<h4>void addContact(struct Contact contacts[], int size);</h4>

<ul>

 <li><strong>addContact</strong> does not return a value and receives a <strong>Contact</strong> array, and an integer for parameters.</li>

 <li>The details on how this function should work is described in Milestone 4.</li>

</ul>

<h4>void updateContact(struct Contact contacts[], int size);</h4>

<ul>

 <li><strong>updateContact</strong> does not return a value and receives a <strong>Contact</strong> array, and an integer for parameters.</li>

 <li>The details on how this function should work is described in Milestone 4.</li>

</ul>

<h4>void deleteContact(struct Contact contacts[], int size);</h4>

<ul>

 <li><strong>deleteContact</strong> does not return a value and receives a <strong>Contact</strong> array, and an integer for parameters.</li>

 <li>The details on how this function should work is described in Milestone 4.</li>

</ul>

<h4>void sortContacts(struct Contact contacts[], int size);</h4>

<ul>

 <li><strong>sortContacts</strong> does not return a value and receives a <strong>Contact</strong> array, and an integer for parameters.</li>

 <li>The details on how this function should work is described in Milestone 4. <strong><u>Contact Helper Source File</u></strong><strong> (.c)</strong></li>

</ul>

Open the <strong>contactHelpers.c</strong> source code file.

<h3>Libraries</h3>

Include the system library <strong>&lt;string.h&gt;</strong> (refer to the source comments for placement).  This library contains the needed string related functions you will use in some of the new functions.  Be sure to also include the <strong>contactHelpers.h</strong> header file.

<h3>Function Definitions</h3>

Function getTenDigitPhone is mostly defined for you (see below for the details), but <strong>requires some modifications</strong>:

<h4>void getTenDigitPhone(char phoneNum[]);</h4>

<ul>

 <li><strong>getTenDigitPhone</strong> does not return a value and expects a C string character array sized for 10 characters (plus the null terminator).</li>

 <li>This function receives user input for a 10-digit phone number and stores the value to the parameter <strong>phoneNum</strong>.</li>

</ul>

<table width="473">

 <tbody>

  <tr>

   <td width="473"> <strong><u>Reminder</u></strong><strong>   </strong><em>Arrays by variable name (ex: phoneNum) is a pointer type (points to the 1<sup>st</sup> element).  This means any changes made using this variable will directly update the source it points to. </em></td>

  </tr>

 </tbody>

</table>

<ul>

 <li>If the entered value is not 10 characters in length or if it does not contain all numeric characters, a message is displayed and continues to prompt until a 10 character C string containing all numeric characters is entered:</li>

</ul>




&gt;Enter a 10-digit phone number: &lt;




<ul>

 <li>This function provides a failsafe method in receiving a 10-digit character C string array.</li>

 <li><strong><u>NOTE</u></strong><strong>: </strong>You need to modify this function to ensure all values entered are <strong><u>numerical</u> <u>digits</u> (this will be tested in milestone 4)</strong></li>

</ul>




Just as you did in MS1, add an empty function definition for all the new functions prototyped in the <strong>contactHelpers.h</strong> header file.  To help you get going, findContactIndex is done for you.  Use the provided source code comments for placement.

<h4><u>Contacts Header File</u> (.h)</h4>

Open the header file <strong>contacts.h</strong>.  There are a few additional lines of code added to the top and bottom areas of the file:




#ifndef CONTACTS_H_

#define CONTACTS_H_




// Header file contents…




#endif // !CONTACTS_H_




<h5>Brief Explanation</h5>

<em>These lines of code “<strong>safeguard</strong>” the header file to ensure it is only included once when the application is compiled (when it is included multiple times by other files).  This is an advanced topic not covered in this course but will be covered in the next level course C++ (OOP244/BTP200). </em>

<strong> </strong>

Refer to the comments in the <strong>contacts.h</strong> file and carefully insert your code from MS2 where directed.




There are no further modifications to make to this file for this milestone.

<h4><u>Contacts Source File</u> (.c)</h4>

The addition of the new helper function getTenDigitPhone, would benefit the getNumbers function in this module.

Copy your MS2 code where the comments indicate.  Update the getNumbers function to use the new function getTenDigitPhone where appropriate to ensure a 10-digit character value is stored for the numbers.




<table width="623">

 <tbody>

  <tr>

   <td width="53"><strong><u>Hint</u></strong><strong>:</strong> </td>

   <td width="569">The getTenDigitPhone function <strong>does not display an initial prompt message</strong>.  The function will display a generic prompt only when and if an invalid value is entered.  You should first display the prompt message specific to the case, then call the getTenDigitPhone function:char examplePhone[11];printf(“Enter example phone number: “);getTenDigitPhone(examplePhone);</td>

  </tr>

 </tbody>

</table>




<h3>Milestone 3 Submission</h3>

Milestone 3 is to be done in the lab and shown to your instructor, there is no need to submit on matrix.

<h2>Milestone 4 (20%)</h2>

<h3>(Due Four (4) days from assigned date)</h3>

Open the project file <strong>A2MS4</strong> and look inside (expand “Header Files” and “Source Files” folders – see figure 2.4.1).  Do not modify the source code file:  <strong>a2ms4.c</strong>.  This is the main file used to assess your functions to determine if they work to this milestone’s specifications.







<u>Figure</u>: 2.4.1 – Visual Studio Project Contents




<h3><u>Unchanged Files</u></h3>

<strong> </strong>

<strong>contacts.h contacts.c </strong>

<strong>contactHelpers.h</strong>




Open each of these files in the provided project.  Consult the comments provided and copy the appropriate contents from Milestone 3.







<h3><u>Contact Helper Source File</u> (.c)</h3>

<ol>

 <li>Open the <strong>c</strong> source code file.</li>

 <li>Define MAXCONTACTS 5 where the comments indicate (under the include section). This will be used for sizing the contacts array later in the program</li>

 <li>Copy the contents from MS3 where the comments indicate.</li>

 <li>Complete the full function definitions for each function using the descriptions below:</li>

</ol>

<strong>Function Definitions</strong> <strong>void</strong><strong> getTenDigitPhone(</strong><strong>char </strong><strong>phoneNum[]); </strong>

<ul>

 <li><strong><u>Modify</u></strong> this function to ensure all values entered are <strong><u>numerical digits</u></strong></li>

</ul>




<h4>int findContactIndex(const struct Contact contacts[], int size,                                              const char cellNum[]);</h4>

<ul>

 <li><strong>findContactIndex</strong> returns an integer and expects a <strong>Contact</strong> array (marked constant so changes can’t be made to it), and integer (intended for representing the size of the Contact array), and a character array (expecting a C string representing a cell phone number).</li>

 <li>This function’s purpose is to find a contact based on the provided cell phone number (parameter 3) and return the index (position in the array) otherwise, if the contact is not found, the function should return -1</li>

</ul>

<strong><u>Hints</u></strong>

<ul>

 <li><em>Iterate the Contact array (up to the size specified in parameter-2) and compare the current iteration contact’s cell phone number to the parameter-3 cell phone number to determine equality </em></li>

 <li><em>Use a <strong>string library function</strong> for string compare</em></li>

</ul>

<strong> </strong>

<h4>void displayContactHeader(void);</h4>

<ul>

 <li><strong>displayContactHeader </strong>does not return a value and has no parameters.</li>

 <li>This function display’s a centered title “Contacts Listing” header that is surrounded in a border:</li>

</ul>

+—————————————————————————–+ [line-1] |                              Contacts Listing                               | [line-2]

+—————————————————————————–+ [line-3]




<strong>Line-1 and Line-3:</strong>

<strong>‘+’</strong> one (1) plus symbol

<strong>‘-‘</strong> seventy-seven (77) minus symbols

<strong>‘+’</strong> one (1) plus symbol

Followed by a newline ‘
’




<strong>Line-2: </strong>

‘|’ one (1) vertical pipe symbol (usually located above the enter key)

‘ ‘ thirty (30) spaces

‘Contacts Listing’ (the title)

‘ ‘ thirty (31) spaces

‘|’ one plus symbol

<h4>Followed by a newline ‘
’ void displayContactFooter(int count);</h4>

<ul>

 <li><strong>displayContactFooter</strong> does not return a value and receives one integer parameter.</li>

 <li>This function display’s a line and a total contact summary</li>

 <li>The function parameter is the total number of contacts value to display</li>

</ul>

+—————————————————————————–+ [line-1] Total contacts: 99    [line-2]




<strong>Line-1:</strong>

<strong>‘+’</strong> one (1) plus symbol

<strong>‘-‘</strong> seventy-seven (77) minus symbols

<strong>‘+’</strong> one (1) plus symbol Followed by a newline ‘
’

<strong>Line-2:</strong>

<strong>‘Total contacts: ‘</strong> Note: one (1) space after the colon

Followed by the integer parameter value Followed by <u>TWO</u> (2) newlines (‘
’)

<h4>void displayContact(const struct Contact *contact);</h4>

<ul>

 <li><strong>displayContact</strong> does not return a value and receives a constant <strong>Contact</strong> pointer (cannot be updated) parameter.</li>

 <li>This function displays the details for a single contact (see example below):</li>

</ul>

<em>Example: With middle initial and an apartment number: </em>

Maggie R. Greene                                             [line-1]

C: 9051112222   H: 9052223333   B: 9053334444             [line-2]        55 Hightop House, Apt# 201, Bolton, A9A 3K3            [line-3]

<em>Example: <u>No middle initial</u> and <u>no apartment number</u>: </em>

Maggie Greene                                                [line-1]

C: 9051112222   H: 9052223333   B: 9053334444             [line-2]        55 Hightop House, Bolton, A9A 3K3                      [line-3]

<strong>Line-1 (contact full name):</strong>

<strong>‘ ‘</strong> one (1) blank space followed by…

<strong>‘Contact full name’</strong> (See below for details) followed by… One (1) newline ‘
’

<u>Contact Full Name</u>:

<ul>

 <li>Consists of all the name parts put together separated by a space</li>

 <li>If there is no middle initial then there should only be one (1) space separating the first name and the last name</li>

</ul>

<strong> </strong>

<strong>Line-2 (contact numbers):</strong>

Use the following format string:

”    C: %-10s   H: %-10s   B: %-10s
” (Note: 4 spaces at the beginning)

<ul>

 <li>The 1<sup>st</sup> specifier is for the cell phone number</li>

 <li>The 2<sup>nd</sup> specifier is for the home phone number</li>

 <li>The 3<sup>rd</sup> specifier is for the business phone number</li>

</ul>




<strong>Line-3 (contact address):</strong>

Use the following format string to get started: ”       %d %s, ” (Note: 7 spaces at the beginning and 1 after the comma)

<ul>

 <li>The 1<sup>st</sup> specifier is for the street number</li>

 <li>The 2<sup>nd</sup> specifier is for the street name</li>

</ul>

<strong> </strong>

<strong><u>IF</u></strong> the apartment field has a value (will be &gt; 0) then include on the same line:

“Apt# %d, ” (Note: 1 space after the comma) – The specifier is for the apartment number

Followed by the city and postal code comma separated:

“%s, %s
”

<ul>

 <li>The 1<sup>st</sup> specifier is for the city</li>

 <li>The 2<sup>nd</sup> specifier is for the postal code</li>

</ul>

<h4>void displayContacts(const struct Contact contacts[], int size);</h4>

<ul>

 <li><strong>displayContacts</strong> does not return a value and receives a constant <strong>Contact</strong> array (cannot be updated), and an integer (intended for representing the size of the Contact array).</li>

 <li>This function needs to display a title header, a detail listing of each <strong>VALID</strong> contact in the array and a footer section showing the total number of contacts.</li>

 <li>To produce the title header, call the displayHeader function described earlier in this milestone</li>

 <li>You will need to iterate all items in the <strong>Contact</strong> array (parameter 1) up to the number of items it holds (parameter 2).</li>

 <li><strong><u>IF</u></strong> the current iterator <strong>Contact</strong> is <strong>VALID</strong> (will have a cell number &gt; 0), display the details (call the displayContact function described earlier in this milestone).</li>

 <li>After iterating all the contacts, finish with displaying the footer summary section by calling the displayContactFooter</li>

</ul>




<strong><u>Hint</u></strong><strong>:</strong> Keep track of the number of valid contacts displayed and pass this count to the displayContactFooter function

<h4>void searchContacts(const struct Contact contacts[], int size);</h4>

<ul>

 <li><strong>searchContacts</strong> does not return a value and receives a constant <strong>Contact</strong> array (cannot be updated), and an integer (intended for representing the size of the Contact array).</li>

 <li>This function should prompt the user to search the contact listings based on a cell phone number. If there is a match, display the details for the contact.</li>

 <li>Prompt the user for a cell phone number to search:</li>

</ul>

&gt;Enter the cell number for the contact: &lt;

–    Do not allow the application to continue until a 10-digit phone is entered.

(<strong>Hint</strong>: call the getTenDigitPhone function to get the value)

<ul>

 <li>Search the contact array to find a contact with the cell phone number previously entered (<strong>Hint</strong>: call function findContactIndex)</li>

 <li>If the contact is found, display the details (<strong>Hint</strong>: call function displayContact) <strong>Note</strong>: follow with one (1) newline (‘
’)</li>

 <li>Otherwise, show the following message:</li>

</ul>

<h4>&gt;*** Contact NOT FOUND ***&lt; (add a newline ‘
’) void addContact(struct Contact contacts[], int size);</h4>

<ul>

 <li><strong>addContact</strong> does not return a value and receives a <strong>Contact</strong> array, and an integer (intended for representing the size of the Contact array).</li>

 <li>This function should first determine if there is an available slot (empty index) in the contact array. This requires iterating the contact array and looking for the first available element having a cell number string length equal to zero (0).  <strong><u>Hint</u></strong>: use the findContact function providing an empty <em>cellNumber</em></li>

 <li>If there are no available slots, the contact listing is full. Notify the user displaying the following message:</li>

</ul>

&gt;*** ERROR: The contact list is full! ***&lt; (add a newline ‘
’)

<ul>

 <li>Otherwise, prompt the user to enter the details for the new contact (store to the contact array at the determined empty slot index). <strong><u>Hint</u></strong>:  use the getContact function</li>

 <li>After adding the new contact, display the following message:</li>

</ul>

<h4>&gt;— New contact added! —&lt; (add a newline ‘
’) void updateContact(struct Contact contacts[], int size);</h4>

<ul>

 <li><strong>updateContact</strong> does not return a value and receives a <strong>Contact</strong> array, and an integer (intended for representing the size of the Contact array).</li>

 <li>This function should prompt the user for the cell phone number of the contact to update.</li>

 <li>Search the contact array to find a contact with the cell phone number previously entered. <strong><u>Hint</u></strong>: call the findContactIndex function</li>

 <li>If the contact could NOT be located, display the following message:</li>

</ul>

&gt;*** Contact NOT FOUND ***&lt; (add a newline ‘
’)

<ul>

 <li>Otherwise, if the contact is located, display the following message:</li>

</ul>

Print a newline (‘
’) followed by:

&gt;Contact found:&lt;

Follow with another newline (‘
’)

<ul>

 <li>Then display the details for the contact. <strong><u>Hint</u></strong>: call the displayContact function – followed by a newline (‘
’)</li>

 <li>Prompt the user with the following message:</li>

</ul>

&gt;Do you want to update the name? (y or n): &lt;  <strong><u>Hint</u></strong>: call the yes function

<ul>

 <li>If the user responds yes (‘y’|’Y’) call the function getName to update the name member of the contact</li>

</ul>

<ul>

 <li>Follow with a prompt displaying the following message:</li>

</ul>

&gt;Do you want to update the address? (y or n): &lt;  <strong><u>Hint</u></strong>: call the yes function

<ul>

 <li>If the user responds yes (‘y’|’Y’) call the function getAddress to update the address member of the contact</li>

</ul>

<ul>

 <li>Follow with a prompt displaying the following message:</li>

</ul>

&gt;Do you want to update the numbers? (y or n): &lt;  <strong><u>Hint</u></strong>: call the yes function

<ul>

 <li>If the user responds yes (‘y’|’Y’) call the function getNumbers to update the numbers member of the contact</li>

</ul>

<ul>

 <li>Lastly display a confirmation message to indicate the contact information was updated:</li>

</ul>

&gt;— Contact Updated! —&lt; (add a newline ‘
’)

<h4> void deleteContact(struct Contact contacts[], int size);</h4>

<ul>

 <li><strong>deleteContact</strong> does not return a value and receives a <strong>Contact</strong> array, and an integer (intended for representing the size of the Contact array).</li>

 <li>This function should prompt the user for the cell phone number of the contact to delete from the list.</li>

 <li>Search the contact array to find a contact with the cell phone number previously entered. <strong><u>Hint</u></strong>: call the findContactIndex function</li>

 <li>If the contact could NOT be located, display the following message:</li>

</ul>

&gt;*** Contact NOT FOUND ***&lt; (add a newline ‘
’)

<ul>

 <li>Otherwise, if the contact is located, display the following message:</li>

</ul>

Print a newline (‘
’) followed by:

&gt;Contact found:&lt;

Follow with another newline (‘
’)

<ul>

 <li>Then display the details for the contact. <strong><u>Hint</u></strong>: call the displayContact function – followed by a newline (‘
’)</li>

 <li>Prompt the user with the following message:</li>

</ul>

&gt;CONFIRM: Delete this contact? (y or n): &lt;  <strong><u>Hint</u></strong>: call the yes function – If the user responds yes, set the contact’s cell number to an empty string (Hint:

assign a null terminator character to the first element)

<ul>

 <li>Lastly display a confirmation message to indicate the contact was deleted: &gt;— Contact deleted! —&lt; (add a newline ‘
’)</li>

</ul>

<strong> </strong>

<table width="574">

 <tbody>

  <tr>

   <td width="574"><strong><u>NOTE</u></strong><strong>   </strong><em>The <strong>sortContacts</strong> function is </em><strong><em>OPTIONAL</em></strong> <em>(<strong>unless otherwise specified by your instructor</strong>) </em><em>If you successfully define this function (and if your instructor does not <u>require</u> you to do this function), <strong>bonus marks will be given</strong> to compensate your extra effort. </em><em><u>If you chose NOT to do this function</u></em><em>, display the following message: </em><strong>&gt;</strong>&lt;&lt;&lt; Feature to sort is unavailable &gt;&gt;&gt;<strong>&lt; </strong>(add a newline ‘
’)</td>

  </tr>

 </tbody>

</table>

<h4>void sortContacts(struct Contact contacts[], int size);</h4>

<ul>

 <li><strong>sortContacts</strong> does not return a value and receives a <strong>Contact</strong> array, and an integer (intended for representing the size of the Contact array).</li>

 <li>This function reorders the elements in the contacts array from lowest to highest based on the cell phone numbers.</li>

 <li>After sorting is done (the array is reordered), display the following message:</li>

</ul>

&gt;— Contacts sorted! —&lt; (add a newline ‘
’)

<ul>

 <li><strong><u>Hint</u></strong>: Review the course notes on Algorithms (specifically the sections on “<strong>Sorting</strong>”)</li>

</ul>




<ol start="5">

 <li>Lastly, revise the contactManagerSystem function.</li>

</ol>

<ul>

 <li>Create a <strong>Contact</strong> array sized to MAXCONTACTS and provide it a meaningful name.</li>

</ul>

–     Initialize the array to hold the following:

{ { { “Rick”, {‘ ’}, “Grimes” },

{ 11, “Trailer Park”, 0, “A7A 2J2”, “King City” },

{ “4161112222”, “4162223333”, “4163334444” } },

{

{ “Maggie”, “R.”, “Greene” },

{ 55, “Hightop House”, 0, “A9A 3K3”, “Bolton” },

{ “9051112222”, “9052223333”, “9053334444” } },

{

{ “Morgan”, “A.”, “Jones” },

{ 77, “Cottage Lane”, 0, “C7C 9Q9”, “Peterborough” },

{ “7051112222”, “7052223333”, “7053334444” } },

{

{ “Sasha”, {‘ ’}, “Williams” },

{ 55, “Hightop House”, 0, “A9A 3K3”, “Bolton” },

{ “9052223333”, “9052223333”, “9054445555” } },     };

<ul>

 <li>Next, refer to the below for what function should be called for each menu selection:</li>

</ul>




<table width="496">

 <tbody>

  <tr>

   <td width="318">Contact Management System————————-</td>

   <td width="178"></td>

  </tr>

  <tr>

   <td width="318">1. Display contacts</td>

   <td width="178"><em>C</em><em>all function: </em><strong><em>displayContacts</em></strong></td>

  </tr>

  <tr>

   <td width="318">2. Add a contact</td>

   <td width="178"><em>C</em><em>all function: </em><strong><em>addContact</em></strong></td>

  </tr>

  <tr>

   <td width="318">3. Update a contact</td>

   <td width="178"><em>C</em><em>all function: </em><strong><em>updateContact</em></strong></td>

  </tr>

  <tr>

   <td width="318">4. Delete a contact</td>

   <td width="178"><em>C</em><em>all function: </em><strong><em>deleteContact</em></strong></td>

  </tr>

  <tr>

   <td width="318">5. Search contacts by cell phone number</td>

   <td width="178"><em>C</em><em>all function: </em><strong><em>searchContacts</em></strong></td>

  </tr>

  <tr>

   <td width="318">6. Sort contacts by cell phone number0. Exit</td>

   <td width="178"><em>C</em><em>all function: </em><strong><em>sortContacts</em></strong></td>

  </tr>

 </tbody>

</table>




Select an option:&gt;

<h2>Sample Output (<u>NO</u> Sorting Option)</h2>

Below is a sample output.  User input values are identified in <strong>BOLD</strong>.  Your output should match exactly:

——————————————

Testing: Final A#2-Milestone #4

——————————————

Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>7</strong>

*** OUT OF RANGE *** &lt;Enter a number between 0 and 6&gt;:<strong> 1</strong>




+—————————————————————————–


|                              Contacts Listing                               | +—————————————————————————–+  Rick Grimes

C: 4161112222   H: 4162223333   B: 4163334444

11 Trailer Park, King City, A7A 2J2

Maggie R. Greene

C: 9051112222   H: 9052223333   B: 9053334444

55 Hightop House, Bolton, A9A 3K3  Morgan A. Jones

C: 7051112222   H: 7052223333   B: 7053334444

77 Cottage Lane, Peterborough, C7C 9Q9  Sasha Williams

C: 9052223333   H: 9052223333   B: 9054445555

55 Hightop House, Bolton, A9A 3K3 +—————————————————————————–+ Total contacts: 4




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>2</strong>




Please enter the contact’s first name: <strong>I Should</strong>

Do you want to enter a middle initial(s)? (y or n): <strong>y n</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>yes</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>y</strong>

Please enter the contact’s middle initial(s): <strong>Not Be</strong>

Please enter the contact’s last name: <strong>In This List</strong>

Please enter the contact’s street number: <strong>-77</strong>

*** INVALID STREET NUMBER *** &lt;must be a positive number&gt;: <strong>77</strong>

Please enter the contact’s street name: <strong>Cityscape Rd.</strong>

Do you want to enter an apartment number? (y or n): <strong>no</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>n y</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>y</strong>

Please enter the contact’s apartment number: <strong>bison</strong>

*** INVALID INTEGER *** &lt;Please enter an integer&gt;: <strong>-1200</strong>

*** INVALID APARTMENT NUMBER *** &lt;must be a positive number&gt;: <strong>1200</strong>

Please enter the contact’s postal code: <strong>Q8Q 3J3 P3P</strong>

Please enter the contact’s city: <strong>Somewhere City</strong>

Please enter the contact’s cell phone number: <strong>111b223333</strong>

Enter a 10-digit phone number: <strong>1112223333</strong>

Do you want to enter a home phone number? (y or n): <strong>y n</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>N</strong>

Do you want to enter a business phone number? (y or n): <strong>yes</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>y</strong>

Please enter the contact’s business phone number: <strong>222-333-4444</strong>

Enter a 10-digit phone number: <strong>2223334444</strong>

— New contact added! —




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>1</strong>




+—————————————————————————–


|                              Contacts Listing                               | +—————————————————————————–+  Rick Grimes

C: 4161112222   H: 4162223333   B: 4163334444

11 Trailer Park, King City, A7A 2J2

Maggie R. Greene

C: 9051112222   H: 9052223333   B: 9053334444

55 Hightop House, Bolton, A9A 3K3  Morgan A. Jones

C: 7051112222   H: 7052223333   B: 7053334444

77 Cottage Lane, Peterborough, C7C 9Q9  Sasha Williams

C: 9052223333   H: 9052223333   B: 9054445555

55 Hightop House, Bolton, A9A 3K3

I Should Not Be In This List

C: 1112223333   H:              B: 2223334444

77 Cityscape Rd., Apt# 1200, Somewhere City, Q8Q 3J3

+—————————————————————————–+ Total contacts: 5




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>2</strong>




*** ERROR: The contact list is full! ***




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>3</strong>




Enter the cell number for the contact: <strong>6665555</strong>

Enter a 10-digit phone number: <strong>6665551111</strong>

*** Contact NOT FOUND ***




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>3</strong>




Enter the cell number for the contact: <strong>9051112222</strong>




Contact found:

Maggie R. Greene

C: 9051112222   H: 9052223333   B: 9053334444

55 Hightop House, Bolton, A9A 3K3




Do you want to update the name? (y or n): <strong>yes no</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>y</strong>

Please enter the contact’s first name: <strong>Maggie</strong> Do you want to enter a middle initial(s)? (y or n): <strong>y</strong>

Please enter the contact’s middle initial(s): <strong>R.</strong>

Please enter the contact’s last name: <strong>Greene Grimes</strong>

Do you want to update the address? (y or n): <strong>y</strong>

Please enter the contact’s street number: <strong>55</strong>

Please enter the contact’s street name: <strong>Hightop House</strong>

Do you want to enter an apartment number? (y or n): <strong>y</strong>

Please enter the contact’s apartment number: <strong>222</strong>

Please enter the contact’s postal code: <strong>A9A 3K3 </strong>

Please enter the contact’s city: <strong>Bolton</strong>

Do you want to update the numbers? (y or n): <strong>y</strong>

Please enter the contact’s cell phone number:

<table width="76">

 <tbody>

  <tr>

   <td colspan="2" width="76"></td>

  </tr>

  <tr>

   <td colspan="2" width="76"><strong>9051112222</strong></td>

  </tr>

  <tr>

   <td width="50"><strong> </strong></td>

   <td width="26"><strong>n</strong></td>

  </tr>

 </tbody>

</table>

Do you want to enter a home phone number? (y or n):

Do you want to enter a business phone number? (y or n): <strong>n</strong>

— Contact Updated! —




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>1</strong>




+—————————————————————————–


|                              Contacts Listing                               | +—————————————————————————–+  Rick Grimes

C: 4161112222   H: 4162223333   B: 4163334444

11 Trailer Park, King City, A7A 2J2

Maggie R. Greene Grimes

C: 9051112222   H:              B:

55 Hightop House, Apt# 222, Bolton, A9A 3K3  Morgan A. Jones

C: 7051112222   H: 7052223333   B: 7053334444

77 Cottage Lane, Peterborough, C7C 9Q9  Sasha Williams

C: 9052223333   H: 9052223333   B: 9054445555

55 Hightop House, Bolton, A9A 3K3

I Should Not Be In This List

C: 1112223333   H:              B: 2223334444

77 Cityscape Rd., Apt# 1200, Somewhere City, Q8Q 3J3 +—————————————————————————–+ Total contacts: 5




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>4</strong>




Enter the cell number for the contact: <strong>4161112222</strong>




Contact found:  Rick Grimes

C: 4161112222   H: 4162223333   B: 4163334444

11 Trailer Park, King City, A7A 2J2




CONFIRM: Delete this contact? (y or n): <strong>n</strong>




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>4</strong>




Enter the cell number for the contact: <strong>4161112222</strong>




Contact found:  Rick Grimes

C: 4161112222   H: 4162223333   B: 4163334444

11 Trailer Park, King City, A7A 2J2




CONFIRM: Delete this contact? (y or n): <strong>y</strong>

— Contact deleted! —




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>1</strong>




+—————————————————————————–


|                              Contacts Listing                               |

+—————————————————————————–


Maggie R. Greene Grimes

C: 9051112222   H:              B:

55 Hightop House, Apt# 222, Bolton, A9A 3K3  Morgan A. Jones

C: 7051112222   H: 7052223333   B: 7053334444

77 Cottage Lane, Peterborough, C7C 9Q9  Sasha Williams

C: 9052223333   H: 9052223333   B: 9054445555

55 Hightop House, Bolton, A9A 3K3

I Should Not Be In This List

C: 1112223333   H:              B: 2223334444

77 Cityscape Rd., Apt# 1200, Somewhere City, Q8Q 3J3

+—————————————————————————–+ Total contacts: 4




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>2</strong>




Please enter the contact’s first name: <strong>Daryl</strong>

Do you want to enter a middle initial(s)? (y or n): <strong>n</strong>

Please enter the contact’s last name: <strong>Dixon</strong>

Please enter the contact’s street number: <strong>11</strong>

Please enter the contact’s street name: <strong>Forest Road</strong>

Do you want to enter an apartment number? (y or n): <strong>n</strong>

Please enter the contact’s postal code: <strong>Y2Y 2N2</strong>

Please enter the contact’s city: <strong>The Kingdom</strong>

Please enter the contact’s cell phone number: <strong>9993338888</strong>

Do you want to enter a home phone number? (y or n): <strong>n</strong>

Do you want to enter a business phone number? (y or n): <strong>n</strong>

— New contact added! —




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>1</strong>




+—————————————————————————–


|                              Contacts Listing                               | +—————————————————————————–+  Daryl Dixon

C: 9993338888   H:              B:

11 Forest Road, The Kingdom, Y2Y 2N2

Maggie R. Greene Grimes

C: 9051112222   H:              B:

55 Hightop House, Apt# 222, Bolton, A9A 3K3  Morgan A. Jones

C: 7051112222   H: 7052223333   B: 7053334444

77 Cottage Lane, Peterborough, C7C 9Q9  Sasha Williams

C: 9052223333   H: 9052223333   B: 9054445555

55 Hightop House, Bolton, A9A 3K3

I Should Not Be In This List

C: 1112223333   H:              B: 2223334444

77 Cityscape Rd., Apt# 1200, Somewhere City, Q8Q 3J3

+—————————————————————————–+ Total contacts: 5




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————-

<ol>

 <li>Display contacts 2. Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>3</strong>




Enter the cell number for the contact: <strong>1112223333</strong>




Contact found:

I Should Not Be In This List

C: 1112223333   H:              B: 2223334444

77 Cityscape Rd., Apt# 1200, Somewhere City, Q8Q 3J3

Do you want to update the name? (y or n): <strong>y</strong>

Please enter the contact’s first name: <strong>Rick</strong>

Do you want to enter a middle initial(s)? (y or n): <strong>n</strong>

Please enter the contact’s last name: <strong>Grimes</strong>

Do you want to update the address? (y or n): <strong>n</strong>

Do you want to update the numbers? (y or n): <strong>n</strong>

— Contact Updated! —




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>1</strong>




+—————————————————————————–


|                              Contacts Listing                               | +—————————————————————————–+  Daryl Dixon

C: 9993338888   H:              B:

11 Forest Road, The Kingdom, Y2Y 2N2

Maggie R. Greene Grimes

C: 9051112222   H:              B:

55 Hightop House, Apt# 222, Bolton, A9A 3K3  Morgan A. Jones

C: 7051112222   H: 7052223333   B: 7053334444

77 Cottage Lane, Peterborough, C7C 9Q9  Sasha Williams

C: 9052223333   H: 9052223333   B: 9054445555

55 Hightop House, Bolton, A9A 3K3

Rick Grimes

C: 1112223333   H:              B: 2223334444

77 Cityscape Rd., Apt# 1200, Somewhere City, Q8Q 3J3

+—————————————————————————–+ Total contacts: 5




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System ————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>

Select an option:&gt;<strong> 5</strong>




Enter the cell number for the contact: <strong>9052223333</strong>




Sasha Williams

C: 9052223333   H: 9052223333   B: 9054445555

55 Hightop House, Bolton, A9A 3K3




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>5</strong>




Enter the cell number for the contact: <strong>9998887777</strong>

*** Contact NOT FOUND ***




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>6 </strong>




&lt;&lt;&lt; Feature to sort is unavailable &gt;&gt;&gt;




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>0</strong>

Exit the program? (Y)es/(N)o: <strong>No yes</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>ny</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;:<strong> n</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>0</strong>




Exit the program? (Y)es/(N)o: <strong>y</strong>




Contact Management System: terminated

<strong> </strong>




<strong>Sample Output (</strong><strong>With Sorting Option</strong><strong>)</strong>

Below is a sample output.  User input values are identified in <strong>BOLD</strong>.  Your output should match exactly:

——————————————

Testing: Final A#2-Milestone #4 (Sort)

——————————————

Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>7</strong>

*** OUT OF RANGE *** &lt;Enter a number between 0 and 6&gt;: <strong>1</strong>




+—————————————————————————–


|                              Contacts Listing                               | +—————————————————————————–+  Rick Grimes

C: 4161112222   H: 4162223333   B: 4163334444

11 Trailer Park, King City, A7A 2J2

Maggie R. Greene

C: 9051112222   H: 9052223333   B: 9053334444

55 Hightop House, Bolton, A9A 3K3  Morgan A. Jones

C: 7051112222   H: 7052223333   B: 7053334444

77 Cottage Lane, Peterborough, C7C 9Q9

Sasha Williams

C: 9052223333   H: 9052223333   B: 9054445555

55 Hightop House, Bolton, A9A 3K3 +—————————————————————————–+ Total contacts: 4




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt;<strong> 2</strong>




Please enter the contact’s first name: <strong>I Should</strong>

Do you want to enter a middle initial(s)? (y or n): <strong>y n</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>yes</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>y</strong>

Please enter the contact’s middle initial(s): <strong>Not Be </strong>

Please enter the contact’s last name: <strong>In This List</strong>

Please enter the contact’s street number: <strong>-77</strong>

*** INVALID STREET NUMBER *** &lt;must be a positive number&gt;: <strong>77</strong>

Please enter the contact’s street name: <strong>Cityscape Rd.</strong>

Do you want to enter an apartment number? (y or n): <strong>no</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>n y</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>y</strong>

Please enter the contact’s apartment number: <strong>bison</strong>

*** INVALID INTEGER *** &lt;Please enter an integer&gt;: <strong>-1200</strong>

*** INVALID APARTMENT NUMBER *** &lt;must be a positive number&gt;: <strong>1200</strong>

Please enter the contact’s postal code: <strong>Q8Q 3J3 P3P</strong>

Please enter the contact’s city: <strong>Somewhere City</strong>

Please enter the contact’s cell phone number: <strong>111b223333</strong>

Enter a 10-digit phone number: <strong>1112223333</strong>

Do you want to enter a home phone number? (y or n): <strong>y n</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>N</strong>

Do you want to enter a business phone number? (y or n): <strong>yes</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>y</strong>

Please enter the contact’s business phone number: <strong>222-333-4444 </strong>

Enter a 10-digit phone number: <strong>2223334444</strong>

— New contact added! —




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>1</strong>




+—————————————————————————–


|                              Contacts Listing                               | +—————————————————————————–+  Rick Grimes

C: 4161112222   H: 4162223333   B: 4163334444

11 Trailer Park, King City, A7A 2J2

Maggie R. Greene

C: 9051112222   H: 9052223333   B: 9053334444

55 Hightop House, Bolton, A9A 3K3  Morgan A. Jones

C: 7051112222   H: 7052223333   B: 7053334444

77 Cottage Lane, Peterborough, C7C 9Q9  Sasha Williams

C: 9052223333   H: 9052223333   B: 9054445555

55 Hightop House, Bolton, A9A 3K3

I Should Not Be In This List

C: 1112223333   H:              B: 2223334444

77 Cityscape Rd., Apt# 1200, Somewhere City, Q8Q 3J3

+—————————————————————————–+ Total contacts: 5




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>2</strong>




*** ERROR: The contact list is full! ***




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>3</strong>




Enter the cell number for the contact: <strong>6665555</strong>

Enter a 10-digit phone number: <strong>6665551111</strong>

*** Contact NOT FOUND ***




(Press Enter to Continue)




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>3</strong>




Enter the cell number for the contact: <strong>9051112222</strong>




Contact found:

Maggie R. Greene

C: 9051112222   H: 9052223333   B: 9053334444

55 Hightop House, Bolton, A9A 3K3




Do you want to update the name? (y or n): <strong>yes no</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>y</strong>

Please enter the contact’s first name: <strong>Maggie</strong> Do you want to enter a middle initial(s)? (y or n): <strong>y</strong>

Please enter the contact’s middle initial(s): <strong>R.</strong>

Please enter the contact’s last name: <strong>Greene Grimes</strong>

Do you want to update the address? (y or n): <strong>y</strong>

Please enter the contact’s street number: <strong>55</strong>

Please enter the contact’s street name: <strong>Hightop House</strong>

Do you want to enter an apartment number? (y or n): <strong>y</strong>

Please enter the contact’s apartment number: <strong>222</strong>

Please enter the contact’s postal code: <strong>A9A 3K3 </strong>

Please enter the contact’s city: <strong>Bolton</strong>

Do you want to update the numbers? (y or n): <strong>y</strong>

Please enter the contact’s cell phone number:

<table width="76">

 <tbody>

  <tr>

   <td colspan="2" width="76"></td>

  </tr>

  <tr>

   <td colspan="2" width="76"><strong>9051112222</strong></td>

  </tr>

  <tr>

   <td width="50"></td>

   <td width="26"><strong>n</strong></td>

  </tr>

 </tbody>

</table>

Do you want to enter a home phone number? (y or n):

Do you want to enter a business phone number? (y or n): <strong>n</strong>

— Contact Updated! —




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>1</strong>




+—————————————————————————–


|                              Contacts Listing                               | +—————————————————————————–+  Rick Grimes

C: 4161112222   H: 4162223333   B: 4163334444

11 Trailer Park, King City, A7A 2J2

Maggie R. Greene Grimes

C: 9051112222   H:              B:

55 Hightop House, Apt# 222, Bolton, A9A 3K3  Morgan A. Jones

C: 7051112222   H: 7052223333   B: 7053334444

77 Cottage Lane, Peterborough, C7C 9Q9  Sasha Williams

C: 9052223333   H: 9052223333   B: 9054445555

55 Hightop House, Bolton, A9A 3K3

I Should Not Be In This List

C: 1112223333   H:              B: 2223334444

77 Cityscape Rd., Apt# 1200, Somewhere City, Q8Q 3J3

+—————————————————————————–+ Total contacts: 5




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>4</strong>




Enter the cell number for the contact: <strong>4161112222</strong>




Contact found:  Rick Grimes

C: 4161112222   H: 4162223333   B: 4163334444

11 Trailer Park, King City, A7A 2J2




CONFIRM: Delete this contact? (y or n): <strong>n</strong>




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>4</strong>




Enter the cell number for the contact: <strong>4161112222</strong>




Contact found:  Rick Grimes

C: 4161112222   H: 4162223333   B: 4163334444

11 Trailer Park, King City, A7A 2J2




CONFIRM: Delete this contact? (y or n): <strong>y</strong> — Contact deleted! —




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>1</strong>




+—————————————————————————–+ |                              Contacts Listing                               | +—————————————————————————–


Maggie R. Greene Grimes

C: 9051112222   H:              B:

55 Hightop House, Apt# 222, Bolton, A9A 3K3

Morgan A. Jones

C: 7051112222   H: 7052223333   B: 7053334444

77 Cottage Lane, Peterborough, C7C 9Q9  Sasha Williams

C: 9052223333   H: 9052223333   B: 9054445555

55 Hightop House, Bolton, A9A 3K3

I Should Not Be In This List

C: 1112223333   H:              B: 2223334444

77 Cityscape Rd., Apt# 1200, Somewhere City, Q8Q 3J3

+—————————————————————————–+ Total contacts: 4




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>2</strong>




Please enter the contact’s first name: <strong>Daryl</strong>

Do you want to enter a middle initial(s)? (y or n): <strong>n</strong>

Please enter the contact’s last name: <strong>Dixon</strong>

Please enter the contact’s street number: <strong>11</strong>

Please enter the contact’s street name: <strong>Forest Road</strong>

Do you want to enter an apartment number? (y or n): <strong>n</strong>

Please enter the contact’s postal code: <strong>Y2Y 2N2 </strong>

Please enter the contact’s city: <strong>The Kingdom</strong>

Please enter the contact’s cell phone number: <strong>9993338888</strong>

Do you want to enter a home phone number? (y or n): <strong>n</strong>

Do you want to enter a business phone number? (y or n): <strong>n</strong>

— New contact added! —




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>1</strong>




+—————————————————————————–


|                              Contacts Listing                               | +—————————————————————————–+  Daryl Dixon

C: 9993338888   H:              B:

11 Forest Road, The Kingdom, Y2Y 2N2

Maggie R. Greene Grimes

C: 9051112222   H:              B:

55 Hightop House, Apt# 222, Bolton, A9A 3K3  Morgan A. Jones

C: 7051112222   H: 7052223333   B: 7053334444

77 Cottage Lane, Peterborough, C7C 9Q9  Sasha Williams

C: 9052223333   H: 9052223333   B: 9054445555

55 Hightop House, Bolton, A9A 3K3

I Should Not Be In This List

C: 1112223333   H:              B: 2223334444

77 Cityscape Rd., Apt# 1200, Somewhere City, Q8Q 3J3

+—————————————————————————–+ Total contacts: 5




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>3</strong>




Enter the cell number for the contact: <strong>1112223333</strong>




Contact found:

I Should Not Be In This List

C: 1112223333   H:              B: 2223334444

77 Cityscape Rd., Apt# 1200, Somewhere City, Q8Q 3J3




Do you want to update the name? (y or n): <strong>y</strong>

Please enter the contact’s first name: <strong>Rick</strong>

Do you want to enter a middle initial(s)? (y or n): <strong>n</strong>

Please enter the contact’s last name: <strong>Grimes</strong>

Do you want to update the address? (y or n): <strong>n</strong>

Do you want to update the numbers? (y or n): <strong>n</strong>

— Contact Updated! —




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>1</strong>




+—————————————————————————–


|                              Contacts Listing                               | +—————————————————————————–+  Daryl Dixon

C: 9993338888   H:              B:

11 Forest Road, The Kingdom, Y2Y 2N2

Maggie R. Greene Grimes

C: 9051112222   H:              B:

55 Hightop House, Apt# 222, Bolton, A9A 3K3  Morgan A. Jones

C: 7051112222   H: 7052223333   B: 7053334444

77 Cottage Lane, Peterborough, C7C 9Q9  Sasha Williams

C: 9052223333   H: 9052223333   B: 9054445555

55 Hightop House, Bolton, A9A 3K3  Rick Grimes

C: 1112223333   H:              B: 2223334444

77 Cityscape Rd., Apt# 1200, Somewhere City, Q8Q 3J3

+—————————————————————————–+ Total contacts: 5




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>5</strong>




Enter the cell number for the contact: <strong>9052223333</strong>




Sasha Williams

C: 9052223333   H: 9052223333   B: 9054445555

55 Hightop House, Bolton, A9A 3K3




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>5</strong>




Enter the cell number for the contact: <strong>9998887777</strong>

*** Contact NOT FOUND ***




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>6</strong>




— Contacts sorted! —




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>1</strong>




+—————————————————————————–


|                              Contacts Listing                               | +—————————————————————————–+  Rick Grimes

C: 1112223333   H:              B: 2223334444

77 Cityscape Rd., Apt# 1200, Somewhere City, Q8Q 3J3  Morgan A. Jones

C: 7051112222   H: 7052223333   B: 7053334444

77 Cottage Lane, Peterborough, C7C 9Q9

Maggie R. Greene Grimes

C: 9051112222   H:              B:

55 Hightop House, Apt# 222, Bolton, A9A 3K3  Sasha Williams

C: 9052223333   H: 9052223333   B: 9054445555

55 Hightop House, Bolton, A9A 3K3

Daryl Dixon

C: 9993338888   H:              B:

11 Forest Road, The Kingdom, Y2Y 2N2

+—————————————————————————–+ Total contacts: 5




(Press Enter to Continue)<strong>     &lt;Enter&gt;</strong>




Contact Management System

————————- 1. Display contacts 2. Add a contact

<ol start="3">

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>0</strong>




Exit the program? (Y)es/(N)o: <strong>No yes</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>ny</strong>

*** INVALID ENTRY *** &lt;Only (Y)es or (N)o are acceptable&gt;: <strong>n</strong>




Contact Management System

————————- 1. Display contacts

<ol start="2">

 <li>Add a contact</li>

 <li>Update a contact</li>

 <li>Delete a contact</li>

 <li>Search contacts by cell phone number</li>

 <li>Sort contacts by cell phone number</li>

 <li>Exit</li>

</ol>




Select an option:&gt; <strong>0</strong>




Exit the program? (Y)es/(N)o: <strong>y</strong>




Contact Management System: terminated










<h3>Milestone 4 Reflectio</h3>

Please provide answers to the following in a text file named <strong>reflect.txt.</strong>

In <u>three</u> or more paragraphs and a <strong><u>minimum</u> of 125 words</strong>, explain what you learned while doing these first two milestones.  In <strong><u>addition to what you learned</u></strong>, <strong>y</strong><strong>our reflection should <u>also include the</u> <u>following</u></strong>:

<ul>

 <li>An explanation of how the two functions <strong>findContactIndex</strong> and <strong>getTenDigitPhone</strong> benefit your source code with respect to overall maintenance and readability.</li>

</ul>




<ul>

 <li>Would you have liked this assignment to include the functionality to load/save the contact information from/to a text data file? Explain your decision.</li>

</ul>

<strong>Reflections will be graded based on the published rubric (</strong><a href="https://github.com/Seneca-144100/IPC-Project/tree/master/Reflection%20Rubric.pdf">https://github.com/Seneca</a><a href="https://github.com/Seneca-144100/IPC-Project/tree/master/Reflection%20Rubric.pdf">144100/IPC-Project/tree/master/Reflection%20Rubric.pdf</a><a href="https://github.com/Seneca-144100/IPC-Project/tree/master/Reflection%20Rubric.pdf"><strong>)</strong></a><strong>.</strong>

<strong><u>Example</u></strong><strong>:  </strong>

<strong>An example reflection answer for <u>Workshop #2</u> is available demonstrating the minimum criteria: </strong><a href="https://github.com/Seneca-144100/IPC-Project/tree/master/Example%20Reflection-WS_2.pdf"><strong>https://github.com/Seneca-144100/IPC-Project/tree/master/Example%20Reflection-WS_2.pdf</strong></a>










<h3>Milestone 4 Submission</h3>

If not on matrix already, upload your <strong>contacts.h</strong>,<strong> contacts.c</strong><strong>,</strong><strong> contactHelpers.h</strong><strong>,</strong><strong> contactHelpers.c</strong><strong>,</strong><strong> a2ms2.c</strong>, and <strong>reflect.txt</strong> files to your matrix account. Compile your code as follows:

<h4>&gt; gcc -Wall -o ms4 contacts.c contactHelpers.c a2ms4.c &lt;ENTER&gt;</h4>

This command will compile your code and name your executable “<strong>ms4</strong>”.  Execute <strong>ms4</strong> and make sure everything works properly.

Then run the following script from your account and follow the instructions (replace profname.proflastname with your professors Seneca userid and <u>replace</u> <strong>NAA</strong> with <u>your</u> section):

<strong>[</strong><strong>NO Sorting Option</strong><strong>] </strong>

<strong>~profname.proflastname/submit 144a2ms4/NAA_ms4 &lt;ENTER&gt;</strong> <strong> </strong>

<h1>&lt;&lt;&lt;  OR  &gt;&gt;&gt;</h1>




<strong>[</strong><strong>WITH Sorting Option</strong><strong>] </strong>

<strong>~profname.proflastname/submit 144a2ms4Sort/NAA_ms4Sort &lt;ENTER&gt;  </strong>




and follow the instructions.

<ul>

 <li></li>

</ul>


