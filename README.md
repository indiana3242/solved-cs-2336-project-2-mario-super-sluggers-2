Download Link: https://assignmentchef.com/product/solved-cs-2336-project-2-mario-super-sluggers-2
<br>
<strong>Pseudocode </strong>

<strong>KEY ITEMS:</strong> Key items are marked in red. Failure to include or complete key items will incur additional deductions as noted beside the item.

<strong>Submission and Grading:</strong>

<ul>

 <li>All project source code will be submitted in zyLabs.

  <ul>

   <li>Projects submitted after the due date are subject to the late penalties described in the syllabus.</li>

  </ul></li>

 <li>Each submitted program will be graded with the rubric provided in eLearning as well as a set of test cases. These test cases will be posted in eLearning after the due date. – zyLabs will provide you with an opportunity to see how well your project works against the test cases. Although you cannot see the actual test cases, a description will be provided for each test case that should help you understand where your program fails.</li>

 <li><strong>Type your name and netID in the comments at the top of all files submitted. (-5 points)</strong></li>

</ul>

<strong>Objective:</strong> Use object-oriented programming to implement and utilize a linked list data structure

<strong>Problem:</strong> Now that the Mushroom Kingdom League has ended and crowned a new champion, it is time to determine the league leaders in several different baseball categories. Being the only person in the Mushroom Kingdom that knows how to write a computer program, you have been asked by Princess Peach herself to write a program that will determine the league leaders.

<strong>Pseudocode:</strong> Your pseudocode should describe the following items

<ul>

 <li>Identify the functions you plan to create for each class

  <ul>

   <li>You do not have to include pseudocode for basic items like constructors, accessors, mutators</li>

  </ul></li>

 <li>For each function, identify the following

  <ul>

   <li>Determine the parameters</li>

   <li>Determine the return type</li>

   <li>Detail the step-by-step logic that the function will perform</li>

  </ul></li>

</ul>

<strong>This will project will extend the basic logic and retain most of the requirements of Project Zero. Differences from Project Zero will be written in blue.</strong>

<strong>Details:</strong>

<ul>

 <li><strong>Classes</strong>

  <ul>

   <li>Use good programming practice for classes – proper variable access, mutators and accessors, proper constructors, etc.</li>

   <li>Remember that classes exist to be used by other people. Just because you don’t use it in the program doesn’t mean it shouldn’t be coded and available for others to use in theirs.</li>

   <li>As with previous projects, you are open to design the classes as you see fit with the minimum requirements listed below</li>

   <li>Both classes must be of your own design and implementation.</li>

  </ul></li>

</ul>

<pre><code>Requirements&#x25aa; Linked list class (-10 points if missing)</code></pre>

<ul>

 <li>Named <strong>LinkList.java</strong></li>

 <li>Members

  <ul>

   <li>Head pointer</li>

   <li>Recursive print function</li>

   <li>A sort function of your own design &#x25aa; Node class</li>

  </ul></li>

 <li>Named <strong>Node.java</strong></li>

 <li>Must be a generic class (-10 points if not)</li>

 <li>Payload variable</li>

 <li>Next pointer &#x25aa; Player class (-5 points if missing)</li>

 <li>Named <strong>Player.java</strong></li>

 <li>Design class to hold stats

  <ul>

   <li>Do not hold stats that are calculated from other stats</li>

   <li>Use functions to calculate when needed</li>

   <li>This prevents stale data</li>

  </ul></li>

 <li>Start the program by prompting the user for the input filename

  <ul>

   <li>This would normally be hardcoded in an application, but zyLabs requires a filename for multiple test files</li>

  </ul></li>

 <li>Nodes will be added to the end of the linked list</li>

 <li>Stats will be calculated for the following categories:

  <ul>

   <li>Batting Average (BA)

    <ul>

     <li>Batting average = hits / at-bats</li>

    </ul></li>

   <li>On-base percentage (OB%)

    <ul>

     <li>On-base percentage = (hits + walks + hit by pitch) / plate appearances</li>

    </ul></li>

   <li>Strikeouts (K)</li>

   <li>Walks (BB)</li>

   <li>Hit by Pitch (HBP)</li>

   <li>Hits (H)</li>

  </ul></li>

 <li>Calculate all stats per person and record the highest value for each category</li>

 <li>There may be ties for the leaders</li>

 <li>If there is a tie, output all names for tied value</li>

 <li>All data must be held and manipulated in a linked list (-10 points if not)</li>

 <li>Any global variables used must be constant</li>

 <li>Use as few variables as possible</li>

</ul>

<strong>Input:</strong> All input will be read from a file. Each player’s data will be listed on separate lines in the file and will follow the same format.

<ul>

 <li>Format:</li>

 <li>Mario HOOKWSHHKOHPWWHO</li>

 <li>The name will be a single word.</li>

 <li>The batting record will be a series of capital letters representing various results during a baseball game

  <ul>

   <li>H – hit</li>

   <li>O – out</li>

   <li>K – strikeout</li>

   <li>W – walk</li>

   <li>P – hit by pitch</li>

   <li>S – sacrifice</li>

  </ul></li>

 <li>Walks, sacrifices and hit by pitches are not considered an at-bat</li>

 <li>Batting records may contain invalid characters.

  <ul>

   <li>If an invalid character is encountered, disregard it</li>

   <li>Invalid characters are not counted as an at-bat</li>

  </ul></li>

 <li>Each line in the file will end in a newline (except the last line of the file which may or may not have a newline)</li>

 <li>The batting record for each person may not have the same number of results</li>

 <li>The input file may have multiple entries for the same person o Combine that data into one node for the player</li>

</ul>

<strong>Output:</strong>

<ul>

 <li>All output will be written to a file – <strong>leaders.txt</strong></li>

 <li>All values are displayed to 3 decimal places</li>

 <li>Display each player’s data in the following order with a tab between each field

  <ul>

   <li>Player name</li>

   <li>At-bats</li>

   <li>Hits</li>

   <li>Walks</li>

   <li>Strikeouts</li>

   <li>Hits by pitch</li>

   <li>Sacrifices</li>

   <li>Batting average</li>

   <li>On-base percentage</li>

   <li>Write a newline after the on-base percentage (there is no tab before the newline)</li>

  </ul></li>

 <li>Output the player data by name in alphabetical order (A to Z)</li>

 <li>After the player data table, display an additional newline and the LEAGUE LEADERS header</li>

 <li>Display the top 3 leaders for each category</li>

 <li>Because of ties all places may not be awarded. o For example, if there is a 3 way tie for first, there would not be a second or third place. o When displaying the leader list, separate each name with a comma and a space</li>

 <li><strong>League Leader Order</strong>

  <ul>

   <li>Batting Average</li>

   <li>On-Base Percentage</li>

   <li>Hits</li>

   <li>Walks</li>

   <li>Strikeouts</li>

   <li>Hit By Pitch</li>

  </ul></li>

 <li><strong>League Leader Output Format</strong>

  <ul>

   <li>CATEGORY newline

    <ul>

     <li>All caps</li>

    </ul></li>

   <li>value _tab_first leader list _newline</li>

   <li>value _tab _second leader list _newline

    <ul>

     <li>Second leader list is optional</li>

     <li>No second place if first place has 3 or more ties</li>

    </ul></li>

   <li>value_tab_third leader list__newline

    <ul>

     <li>Third leader list is optional</li>

     <li>No third place if first or second place has a tie</li>

    </ul></li>

   <li>newline</li>

  </ul></li>

</ul>