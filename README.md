Download Link: https://assignmentchef.com/product/solved-cs240-homework-2-histogram-of-word-lengths
<br>
<h2>1        Histogram of Word Lengths</h2>

Write a C program that reads from stdin till EOF and analyzes the lengths of the words in the input. Let’s consider all alphanumeric characters as words, and all non-alphanumeric characters as delimiters. For example, each of the following is a word.

<ul>

 <li>Homework</li>

 <li>CS240</li>

 <li>2</li>

</ul>

The following strings should be broken into multiple words.

<ul>

 <li>“you’ll” has two words: “you” and “ll”.</li>

 <li>“ALL’S” has two words: “ALL” and “S”.</li>

 <li>“UTF-8” has two words: “UTF” and “8”.</li>

 <li>“2/19/2019 17:00” has five words: “2”, “19”, “2019”, “17”, and “00”.</li>

 <li>“www.gutenberg.org” has three words: “www”, “gutenberg”, and “org”.</li>

</ul>

You can build upon the word counting code on page 20 of K&amp;R. As you read a word one character at a time, keep track the number of characters you have read. When you reach the end of a word, you have its length. Then you increment a counter that keeps track the number of words of this particular length. Use an array of these counters. I will test your code with CompleteShakespeare.txt. The longest word you will encounter has 27 characters.

For output, you should print 27 lines. In each line, you print the length (width 2), a space, the number of words of that length (width 6), a space, and several asterisks. Use one asterisk for each 4,000 words. If there are fewer than 4,000, you still print one asterisk for them, because we cannot print a fractional asterisk. For example, print one asterisk for 1 to 4,000 words, and two asterisks for 4,001 to 8,000 words, and so on. The asterisks constitute the histogram of word lengths. Histograms are usually printed vertically, but here it is printed horizontally because this is easier. On CompleteShakespeare.txt, your code should print exactly like Figure 1.

<ul>

 <li>63691 ****************</li>

 <li>166375 ******************************************</li>

 <li>204211 ****************************************************</li>

 <li>223161 ********************************************************</li>

 <li>121472 *******************************</li>

 <li>80386 *********************</li>

 <li>59379 ***************</li>

 <li>35083 *********</li>

 <li>20351 ******</li>

 <li>10067 ***</li>

 <li>3771 *</li>

 <li>1353 *</li>

 <li>454 *</li>

 <li>247 *</li>

 <li>77 *</li>

 <li>3 *</li>

 <li>4 *</li>

 <li>0</li>

 <li>0</li>

 <li>0</li>

 <li>0</li>

 <li>0</li>

 <li>0</li>

 <li>0</li>

 <li>0</li>

 <li>0</li>

 <li>1 *</li>

</ul>

Figure 1: Output for CompleteShakespeare.txt

<h2>2      Lastly</h2>

Compile and run as follows:

<a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="41343224337971012835322433372433">[email protected]</a>:~/$gcc -Wall histo.c -o histo <a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="22575147501a12624b56514750544750">[email protected]</a>:~/$./histo &lt; CompleteShakespeare.txt

Write plenty of comments to explain your code – how you determine a character is alphanumeric, how you extract one word, and how you convert a count to the number of asterisks to print.

Write a Report.txt that discusses what you found difficult about this assignment, how you planned your approach to it, and what you learned completing it.

Send me only:

<ol>

 <li>c</li>

 <li>txt</li>

</ol>