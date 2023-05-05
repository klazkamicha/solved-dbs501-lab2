Download Link: https://assignmentchef.com/product/solved-dbs501-lab2
<br>
1)  Write the PL/SQL code that may be used as a temperature system converter — you will enter firstly your current (input) scale as C or F and then the value to be converted. The output value should be rounded to only one decimal. Use IF .. THEN logic.             Here are the outputs:




<table>

 <tbody>

  <tr>

   <td>Enter your input scale (C or F) for temperature:</td>

   <td width="12"></td>

   <td></td>

  </tr>

 </tbody>

</table>




<table>

 <tbody>

  <tr>

   <td>Enter your temperature value to be converted:</td>

   <td width="12"></td>

   <td></td>

  </tr>

 </tbody>

</table>

<strong>This is NOT a valid scale. Must be C or F.PL/SQL procedure successfully completed.</strong>

<table>

 <tbody>

  <tr>

   <td width="304">Enter your input scale (C or F) for temperature:</td>

   <td width="12"></td>

   <td width="165"></td>

  </tr>

 </tbody>

</table>




<table>

 <tbody>

  <tr>

   <td>Enter your temperature value to be converted:</td>

   <td width="12"></td>

   <td></td>

  </tr>

 </tbody>

</table>

<strong>Your converted temperature in F is exactly 86PL/SQL procedure successfully completed.</strong>

<table>

 <tbody>

  <tr>

   <td width="304">Enter your input scale (C or F) for temperature:</td>

   <td width="12"></td>

   <td width="165"></td>

  </tr>

 </tbody>

</table>




<table>

 <tbody>

  <tr>

   <td>Enter your temperature value to be converted:</td>

   <td width="12"></td>

   <td></td>

  </tr>

 </tbody>

</table>

<strong>Your converted temperature in C is exactly -31.7PL/SQL procedure successfully completed.</strong>

2)         Write a PL/SQL block that will ask for Instructor’s Id and then will figure out how many sections does teach that person. It will display  then an appropriate  message based on that  number. Use CASE .. WHEN logic.                               Here are the possible outputs:

<table>

 <tbody>

  <tr>

   <td>Please enter the Instructor Id:</td>

   <td width="12"></td>

   <td></td>

  </tr>

 </tbody>

</table>

<strong>This is not a valid instructor </strong>

<table>

 <tbody>

  <tr>

   <td>Please enter the Instructor Id:</td>

   <td width="12"></td>

   <td></td>

  </tr>

 </tbody>

</table>

<strong>Instructor, Tom Wojick, teaches 10 section(s)This instructor needs to rest in the next term.PL/SQL procedure successfully completed.</strong>

<table>

 <tbody>

  <tr>

   <td>Please enter the Instructor Id:</td>

   <td width="12"></td>

   <td></td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong>Instructor, Fernand Hanks, teaches 9 section(s)This instructor teaches enough sections.PL/SQL procedure successfully completed.</strong>




<table>

 <tbody>

  <tr>

   <td>Please enter the Instructor Id:</td>

   <td width="12"></td>

   <td></td>

  </tr>

 </tbody>

</table>

<strong>Instructor, Rick Chow, teaches 0 section(s)This instructor may teach more sections.PL/SQL procedure successfully completed.</strong>

3)         Write a PL/SQL block that will ask for a Positive Integer input and then will calculate the sum of all Even ( or Odd) integers between 1 and that value, depending whether the input value is Even or Odd. Use WHILE LOOP control logic.                         Here are the possible outputs:




<table>

 <tbody>

  <tr>

   <td>Please enter a Positive Integer:</td>

   <td width="12"></td>

   <td></td>

  </tr>

 </tbody>

</table>

<strong>The sum of Even integers between 1 and 12 is 42PL/SQL procedure successfully completed.</strong>

<table>

 <tbody>

  <tr>

   <td>Please enter a Positive Integer:</td>

   <td width="12"></td>

   <td></td>

  </tr>

 </tbody>

</table>

<strong>The sum of Odd integers between 1 and 901 is 203401PL/SQL procedure successfully completed.</strong>

4)         Write a PL/SQL block that will ask for department’s Location Id and then will

figure out how many departments exist there and how many employees work on that location. Based on these answers you will construct a Nested For Loop that will display these answers in a numeric format like shown below. The first location  1800 has only one department with 2 employees, while the other location 1400 has 3 departments with 7 employees altogether (after the Update).

Obviously, without an explicit cursor you can NOT show how many employees works in each department. So, this is just an exercise in creating nested loops.

But, firstly you need to relocate departments 40 and 70 to location 1400.

Do NOT commit, you will rollback it when you finish your block.

UPDATE  Departments   SET   location_id = 1400

WHERE  department_id IN (40,70) ;

<table>

 <tbody>

  <tr>

   <td>Enter valid Location Id:</td>

   <td width="12"></td>

   <td></td>

  </tr>

 </tbody>

</table>

<strong> </strong>

<strong>Outer Loop: Department #1* Inner Loop: Employee #1* Inner Loop: Employee #2PL/SQL procedure successfully completed.</strong>




<table>

 <tbody>

  <tr>

   <td>Enter valid Location Id:</td>

   <td width="12"></td>

   <td></td>

  </tr>

 </tbody>

</table>

<strong>Outer Loop: Department #1* Inner Loop: Employee #1* Inner Loop: Employee #2* Inner Loop: Employee #3* Inner Loop: Employee #4* Inner Loop: Employee #5* Inner Loop: Employee #6* Inner Loop: Employee #7Outer Loop: Department #2* Inner Loop: Employee #1* Inner Loop: Employee #2* Inner Loop: Employee #3* Inner Loop: Employee #4* Inner Loop: Employee #5* Inner Loop: Employee #6* Inner Loop: Employee #7Outer Loop: Department #3* Inner Loop: Employee #1* Inner Loop: Employee #2* Inner Loop: Employee #3* Inner Loop: Employee #4* Inner Loop: Employee #5* Inner Loop: Employee #6* Inner Loop: Employee #7PL/SQL procedure successfully completed.</strong>

ROLLBACK

<strong>Rollback complete.</strong>