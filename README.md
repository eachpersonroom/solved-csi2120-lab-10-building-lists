Download Link: https://assignmentchef.com/product/solved-csi2120-lab-10-building-lists
<br>
This lab explores list which have been covered in detail in the online videos last week. In order to complete the lab, you will need to know:

<ul>

 <li>Scheme uses the same recursive definition of lists as Prolog. What is called the head and tail in Prolog is called the car and cdr in Scheme. (These names come from the original Lisp implementation and stand for “Contents of Address Register” and “Contents of Data Register” referring to some Assembler Macros).</li>

 <li>The main function to build lists is the cons function with makes a pair of a car and cdr.</li>

 <li>The main function to get at the content of lists are the car and cdr.</li>

</ul>

<h3>Exercise 1: Building Lists</h3>

Use cons to build the following lists:

‘(3 4)               ‘(1 2 3)               ‘(a (b c))               ‘(1)               ‘(2 (3 (4)))

<h3>Exercise 2: List Entries</h3>

Use car and cdr to obtain the <em>elements</em> from the list.

;       Example:;       (define L ‘(1 2 3 4 5))    ;;       (car L);       =&gt; 1;;       (cdr L);       =&gt; ‘(2 3 4 5);;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;

Combine calls car and cdr to get the element 2, 3, 4 and 5 from the list L (4 solutions).

;       (define L ‘(1 2 3 4 5))    ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;

Combine calls car and cdr to get the element 2 and 5 from the list LL (2 solutions).

;       (define LL ‘(1 (2 3 4) (5)))    ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;

Note that you can use shorthand commands such

;       (cadr ‘(1 2));       =&gt; 2;       (car (cdr ‘(1 2)));       =&gt; 2    ;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;

<h3>Exercise 3: Integer Range</h3>

Give a function that creates a list with integers in the specified range.

;       The function takes two indices, i and k, and produces the integers;       between i and k including i and k.;;       Example:;       (range 4 9);       =&gt; (4 5 6 7 8 9);;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;

<h3>Exercise 4: Sum of Squares Digit</h3>

Consider the digits d_k,d_(k-1),â€¦,d_1,d_0 of a positive integer number. The squares of the digits are then s = d_k^2 + d_(k-1)^2 + â€¦ + d_1^2 + d_0^2.

Create a function sosd that calculates the sum of square digits.

;   The function calculates the sum of square digits. ;;       Example:;  (sosd 130);       =&gt; 10;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;

<h3>Exercise 5: Every k-th element</h3>

;      The function takes a list and an number selecting every kth;      element. Start counting at 1.;;       Example:;       (drop ‘(a b c d e f g h i k) 3);       =&gt; (a b d e g h k);;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;;

<h3>Exercise 5 and Quiz: List Manipulation</h3>

<em>Please hand-in the answer to this question on Virtual Campus at the latest by Friday 6:00pm! Your submission will only count if you also hand-in solutions to all of the exercises. However, Exercise 1 to 5 will not be graded.</em>

Define a function addSubList that processes a list of lists of numbers and adds up all sub-lists. The output of your function is a flat list of numbers. (You can assume that your function only receives valid input).

(define Q ‘(1 2 (3 4) 1 5 (7 8)));;;;;;;;;;;;;;;;;;;;;; (addSubList Q)      ; =&gt; ‘(1 2 7 1 5 15);;;;;;;;;;;;;;;;;;;