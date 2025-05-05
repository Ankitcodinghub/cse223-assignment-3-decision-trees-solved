# cse223-assignment-3-decision-trees-solved
**TO GET THIS SOLUTION VISIT:** [CSE223 Assignment 3-Decision Trees! Solved](https://www.ankitcodinghub.com/product/cse223-assignment-3-decision-trees-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;95920&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE223 Assignment 3-Decision Trees! Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
.

1 Introduction

For this assignment, you’ll be writing code to implement, use and extend a decision tree. This is similar in spirit to the “20 Questions” game (though we’re not restricting this to 20 questions).

This assignment will be discussed in detail in class, but here are some additional details:

􏰈 you’ll need to implement a binary tree, where each node contains 2 pieces of data: a string of text, and a 􏰇ag indicating whether this is a question or an answer;

􏰈 To play the game, begin at the root (it will be a question), and ask the question;

􏰈 based on the user’s response, travel to the left (YES) or right (NO) sub-tree, and repeat, until you reach an answer;

􏰈 if the answer is correct, no action is necessary;

􏰈 if the answer is wrong, ask for the answer and a new question to discriminate the correct answer from the incorrect one you guessed; then make a new node from that questions and those two answers, and insert it into the tree in place of the incorrect answer.

Additionally, the initial decision tree should be read from a 􏰄le (20Q.txt by default), and, after being modi􏰄ed, re-written to the same 􏰄le. The name of this database should be modi􏰄able by specifying a single command-line argument. Remember to traverse in PRE-ORDER (NLR) to simplify the reading/writing of this 􏰄le.

Here’s a sample initial database 􏰄le:

<pre>Q:
Is it an animal
A:
dog
A:
rock
</pre>
(this 􏰄le should have 6 lines total, with no empty lines).

As always, I strongly recommend approaching this in pieces: make a binary tree class, then

extend it to support this decision tree; then hard-wire some nodes and get it to traverse/play the game. Work on the File I/O separately; work on extending the tree separately; and so on.

1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
You may use built-in primitives from Java such as Scanner, PrintWriter, etc. but create your own tree class, your own 􏰄le parser, your own traversal code, and so on.

Do not use Eclipse, IntelliJ, or any other IDEs: work from the command line on the Linux server (or your own Linux environment). This will ensure you know the syntax for de􏰄ning classes, writing a main method, and so on.

2 Implementation

Make a main method in a class named PA3 (inside a 􏰄le named PA3.java). This should be executable by saying

java PA3

which will read from a database named 􏰁20Q.txt􏰂 (report an error and exit gracefully if it does not exist). Additionally, you can work with a given database by saying

<pre>java PA3 filename
</pre>
which will read from the database named 􏰄lename (and update it as needed) (and again, if the 􏰄le does not exist, report an error and exit gracefully).

This should run your code to play 20 questions, asking the user to think of an item, and then asking questions to guess what the item is. Again, details will be given in class. This is only a high-level overview of the assignment.

If the database 􏰄le exists, you may assume it is a perfect 􏰄le, with the expected structure etc. You are not responsible for handling corrupt 􏰄les.

3 Testing

I have put a pair of databases on the linux server:

/tmp/20Q.txt and /tmp/20QBig.txt

Feel free to copy these into your own directory and work with them there (the copies in /tmp are read-only). 20Q.txt is the sample initial database described above. 20QBig.txt is a larger database holding around 20,000 items (originally given to me by a UW student).

4 Grading

Your assignment must be downloadable from GITLab by me in order to be graded. I will download using the command:

<pre>git clone git@gitlab.com:yourGITid/CSE223PA3.git
</pre>
2

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
You can mimic this yourself to con􏰄rm that your repository is located and named correctly. There’s no sure way to check that you have added me as a reporter: just make sure you do!

Points are awarded as follows:

<ul>
<li>􏰈 &nbsp;Project can be downloaded and compiled: 20 points</li>
<li>􏰈 &nbsp;Program asks questions and makes a guess: 10 points</li>
<li>􏰈 &nbsp;Program acts according to the database 􏰄le (i.e. plays the game as it’s supposed to): 30 points</li>
<li>􏰈 &nbsp;User can specify a di􏰃erent database 􏰄le: 10 points</li>
<li>􏰈 &nbsp;Program updates database 􏰄le if it guesses wrong: 15 points</li>
<li>􏰈 &nbsp;style: 15 points if you have all of the following:
􏰆 consistent indenting, placement of braces, etc.

􏰆 all code commented (every line unless it’s extremely obvious why that line is there) 􏰆 each method described by an introductory block of comments.

􏰆 entire class described by a block of comments in the beginning (in your own words).

5 Submission

Create a repository named CSE223PA3 on GITLab. The repository should contain all of your .java 􏰄les in the top level of the repository. You can include any other 􏰄les, subdirectories, etc. as you like (I will ignore them). Add me (nickmacias) as a reporter on your project.
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</div>
