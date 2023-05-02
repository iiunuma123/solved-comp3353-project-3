Download Link: https://assignmentchef.com/product/solved-comp3353-project-3
<br>
<ul>

 <li>Defining and accessing Arrays.</li>

 <li>Dealing with Registers and instructions.</li>

 <li>Defining with Loops</li>

 <li>Debugging and running your assembly code.</li>

</ul>

<strong><em>Requirements: </em></strong>

<ul>

 <li>Read the design section and write a program. Submit source file (.asm) to Canvas.</li>

 <li>Please start early. ZERO point for late submission. After the <strong>11:59pm </strong>on the due day, you can’t submit your assignment anymore.</li>

</ul>

<strong><em>Deliverables: </em></strong>

<ul>

 <li>Save your source of assembly program as a <strong>.asm </strong></li>

 <li>Name document as a “<strong>asm</strong>”.</li>

 <li>Submit your “<strong>asm</strong>” through the Canvas system. You do not need to submit hard copies.</li>

</ul>

<strong><em>Rebuttal period: </em></strong>

<ul>

 <li>You will be given a period of 3 <strong>business </strong>days to read and respond to the comments and grades of your homework or project assignment. The TA may use this opportunity to address any concern and question you have. The TA also may ask for additional information from you regarding your homework or project.</li>

</ul>

<strong><em>Design: </em></strong>

The objective of this assignment is to create a program that will read a value from an array, and then place this value in another array with the location shifted by a certain amount. The array may be of any length from 2 to 100. Your program must be flexible enough to produce the correct solution regardless of the array size. You must provide documentation for your program in the form of comments.

Create a BYTE array with the label ‘input’. ‘input’ should have eight elements. You should place values 1,2,3,4,5,6,7,8 in each of the elements of this array.

Create a BYTE array with the label ‘output’. This array should be the same length as ‘input’.

Create a DWORD variable with the label ‘shift’. ‘shift’ should hold a single value. The value of ‘shift’ must be less than the length of ‘input’.

The program should then read each of the values from the array ‘input’ and place the values into the ‘output’ array, but the location should be shifted by the amount in the ‘shift’ variable. If the shift would cause a value to be outside of the bounds of ‘output’, then the values should “wrap around” to the front of ‘output’.

Example:

My ‘input’ array is 5, 0A, 2, 6, 0C, 9, 4

‘shift’ is 3

The proper solution for ‘output’ is 0C, 9, 4, 5, 0A, 2, 6

As you can see the value ‘5’ is the 1st value in the ‘input’ array. The value ‘5’ then shifts 3 to the 4th value in the ‘output’ array. Also, note that the value ‘0C’ is the 5th value in the ‘input’ array. After a shift of 3, this would take the value ‘0C’ out of bounds for the ‘output’ array (it is the same length as the ‘input’ array). The value ‘0C’ must “wrap around” to the front of the ‘output’ array. This also holds true for ‘9′ and ‘4’.

Remember that your program must be flexible enough to handle an array of any length.

You are recommended to create a loop to inspect the values in your output array, see page 5 in Debugging_tutorials.pdf for more info.

Header:

Please provide a heading at the top of your code containing your name, Auburn UserID, filename, and how to compile your code.  Also describe any help or sources that you used (as per the syllabus).

e.g. ;Xuechao Li

;Project1.cpp

;Dr. Li helped me debug a syntax error in my “for” loop. ;I used Wikipedia.org to learn how a genetic algorithm works.

;I spoke with Bob Smith in the class about identifying objects in Assembly Language.

Comments

In the coding section, use your judgment to choose between explaining each line or related group of lines. The purpose of these comments is to make the code readable for other programmers or for you in the future.