This assignment consists of 2 problems.

1. Write an awkprogram file named myawkwhich does the followings:
•Display << Startof file >>at the top.
•Display lines between the 3rd line and the 5th line. 
•Display each line backwards, that is, from right to left.
•At the start of each of those lines, display the line number followed by a colon.
•Display << End of file: wordCount = N >> at the end. Here, N must be the number of words betweenline number 3 to 5.

Thus, for the following input text named presents,
Gimme presents I want more!
Gimme presents, I did my chores!
A bicycle, a tricycle, a motor vehicle!
I deserve it, you reserve it!
Gimme presents; more, more, more
Gimme presents I need more!

The output of “awk -f myawk presents” would be
<< Start of file >>
vehicle! motor a tricycle, a bicycle, A
it! reserve you it, deserve I
more more, more, presents; Gimme
<< End of file: wordCount = 18 >>

2. Write a sedprogram file named mysedwhich does the followings:
•Delete lines containing the word more.
•Indent each line with two spaces.
•Enclose each line with << and >>.

Thus, for the following input text named presents,
Gimme presents I want more!
Gimme presents, I did my chores!
A bicycle, a tricycle, a motor vehicle!
I deserve it, you reserve it!Gimme presents; 
more, more, moreGimme presents I need more!

the output of “sed -f mysed presents” would be
<< Gimme presents, I did my chores! >>
<< Abicycle, a tricycle, a motor vehicle! >>
<< I deserve it, you reserve it! >>
