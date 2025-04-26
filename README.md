# ser321-assignment-4--threads-and-serialization-activity-2-solved
**TO GET THIS SOLUTION VISIT:** [SER321 Assignment 4 -Threads and Serialization Activity 2 Solved](https://www.ankitcodinghub.com/product/ser321-assignment-4-threads-and-serialization-activity-2-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;123513&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;SER321 Assignment 4 -Threads and Serialization Activity 2 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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

<div class="kksr-stars-active" style="width: 138px;">
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
            5/5 - (3 votes)    </div>
    </div>
<h1>Prerequisites</h1>
<ol>
<li>The assigned readings in module 4 on Canvas</li>
<li>Lecture videos from Canvas (or in person)</li>
<li>Running and understanding the examples listed on the Canvas page</li>
<li>Setup of a second device (second computer, AWS EC2) – see Canvas for details (should already be done)</li>
</ol>
<strong>Learning outcomes of this assignment are:</strong>

<ol>
<li>Apply sockets in an efficient way</li>
<li>Understand how to use threads</li>
<li>Understand how to work with shared states when using threads</li>
<li>Use different protocols to serialize data</li>
</ol>
<h1>Preliminary things</h1>
I strongly advise you to work on Git and GitHub, to version control and also to practice. Commit whenever something works so you are not losing anything.

Structure: you will have to create two programs one for each Activity. So your assignment 4 folder should have two sub directories (activity1, activity2). Each project needs a README.md and a build.gradle file.

Submit your code and all documents via your GitHub Assignment 4 folder and as a zip on Canvas as usual.

<h1>1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Activity: Threads (30 points)</h1>
<h2>Background</h2>
For this activity you will convert a simple single-threaded server to a multi-threaded server. You will create 2 versions, one that allows threads to grow unbounded, and one that sets the number of allowed clients at a time to a fixed number. This is just a toy example to get started.

You are given starting code of a single-threaded server. There is a Client provided, which you should use for your implementation. The Readme specifies a protocol which you should implement.

<h2>Given Code</h2>
You are given starter code for this assignment on Canvas:

<ul>
<li>java – a main program that accepts incoming client connections</li>
<li>java – a program that does the “business logic” of what the client requests • StringList.java – a simple wrapper class for a list of strings</li>
<li>java – a client which has the main functions and user interaction part which you should implement on the Server/Performer side</li>
<li>A build.gradle file which can run the base Client and Server, see Readme</li>
</ul>
You can have any package structure you want and add new classes etc. Important, you should only have 1 Readme and 1 build.gradle file for all 3 tasks. Each task (server) can be started separately and work only with the features described. You can make any changes in the given files you like, BUT the protocol should work as described in the README.

<h2>Task 1: Make Performer more interesting (8 points)</h2>
Presently, all the Performer does is add strings to the list. Make it more interesting by implementing the protocol described in the Readme. The Client does not have to verify user input, you can assume that when it asks for an int, we will provide an int, etc. The Server however should handle wrong requests and include some error handling, but we will not be mean when testing. You do not have to handle all errors in detail this is more about simple requests and threads. With using things correctly with your Client, things should not crash though! You have some things given but you can make adjustments and add-ons.

<h2>Task 2: Make the server multi-threaded (10 points)</h2>
Create a new Server threaded class “ThreadedServer”. Task 1 should still run as is! So now many Clients should be able to connect to this server and manipulate the list safely.

<ol>
<li>Name this server class “ThreadedServer”</li>
<li>Allow unbounded incoming connections to the server.</li>
<li>No client should block.</li>
<li>The shared state of the string list should be properly managed. Keep the data thread safe.</li>
</ol>
<strong>Task 3: Make the multi-threaded server bounded (4 points) </strong>You can add new classes here of course. Task 1 and 2 should still run as is.

<ol>
<li>Name this server class “ThreadPoolServer”.</li>
<li>Only allow a set number of incoming connections at any given time. How many threads should be specified when calling the program through Gradle.</li>
</ol>
<h2>Gradle (8 points)</h2>
<ol>
<li>(3 points) In your ONE Gradle file there should be 3 Gradle tasks to run the different servers</li>
<li>(1 point) Gradle should use default values for each task, per default host=localhost, port=8000</li>
<li>(1 points) We should be able to run “gradle runClient” and it should use the default values.</li>
<li>Running your different servers with default valued:
<ol>
<li>One for running Task 1: gradle runTask1</li>
<li>One for running Task 2: gradle runTask2</li>
<li>One for running Task 3: gradle runTask3</li>
</ol>
</li>
<li>(1 point) Provide a detailed Readme.md file in your project, which tells us how to run each task and a description of which parts you accomplished of the requirements.</li>
<li>(2 points) Make sure you include your screencast here as well, one screencast for all 3 parts not longer than 4 minutes.</li>
</ol>
<h1>2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Activity: Threads and Protobuf (70 points)</h1>
A simple ’multi-player’ game using Protobuf as protocol.

<h2>The Game</h2>
We want to design and implement a simple modified “version” of the strategy guessing game Battleship. The server will be responsible for handling everything related to the game state and logic. This includes things such as setting and knowing the location of ships on the game board in addition to tracking hits and misses. In this version of the game, players (clients) will be working together to find all of the ships instead of playing against each other.

The server also keeps track of a leaderboard and a log file.

The server and clients communicate through a given Protobuf protocol. See protobuf files and the PROTOCOL.md file in the given code.

<strong>YOU HAVE TO implement the given protocol as described in the PROTOCOL.md with the given proto file!!</strong>

Your code needs to work with our protocol exactly as defined in the .proto file. If you change it, then our client would not work with our server. Theoretically, everyones client should work with everyones server if you impement the given protocol.

See the video on how the game might look like for more detailed information, the video has slight differences and is just to give a general idea, please go by the requirements specified here.

The points in the constraints section add up to more than 70 points. The extra points will be extra credit.

Include a 4min screencast of your game running in your submission and add the link to your README.

<strong>Readme:</strong>

<ol>
<li>(0.5 point) A description of your project and a detailed description of what it does</li>
<li>(0.5 points) An explanation of how we can run the program</li>
<li>(3 points) A short video for each activity (2-4min) showing how you run the program, showing what works and briefly show your code.</li>
<li>(3 points) Name the requirements that you think you fulfilled</li>
</ol>
<h2>Constraints (63 points)</h2>
Server and client should not crash. They should be well implemented, readable, and use good coding practices. If you do not do the above, you might loose points even if the functionality is fulfilled.

Hint: place your project so that there are no whitespaces in the file path. The way files are read right now will not work with whitespaces in the path – you can change that if you like but don’t have to.

<ol>
<li>The project needs to run through Gradle (nothing really to do here, just keep the Gradle file as is)</li>
<li><strong>(6 points) You need to implement the given protocol (Protobuf) see the Protobuf files, the PROTOCOL.md and the Protobuf example in the examples repo (this is NOT an optional requirement)</strong>. If you do not do this you will loose 15 points (instead of getting the 6 points) since then our client will not run your server for testing and thus basically your interface is wrong and not what the customer asked for.</li>
<li>The basic start is given with the client sending over a name to the server and the server responding with a greeting. You continue from there.</li>
<li><strong>(3 points) The main menu gives the user 3 options: 1: leaderboard, 2 play game, 3 quit. After a game is done the menu should pop up again. Implement the menu on the Server side (not optional). </strong>So the menu options are send by the Server to the Client (you should include that in the greeting response).</li>
<li>(3 points) Design your calls and user interaction in a way that they are easy. Remember we have many assignments to grade, design it so it is easy for us. There will be some requirements later you should fulfill.</li>
<li>(2 points) When the user chooses the option 1, a leader board will be shown (does not have to be sorted) or especially pretty when it is shown on the Client terminal.</li>
<li>(2 points) The leaderboard is the same for all clients, take care of multiple clients not overwriting it (keep it thread safe).</li>
<li>(3 points) The leaderboard persists even if the server crashes.</li>
<li>(2 points) The leaderboard keeps track of how many points/wins each player has, in the login field you store how often they logged into the server (so they might show up, even if they did not play). We assume same name equals same player, so you overwrite high scores.</li>
<li>(4 points) Client chooses option 2 (starting a game), then the client sends a start request to the server. The server will respond with a battleship board (either from a running game if one is in progress or a new game) and a flag specifying if it is a new or joined game.</li>
<li>(2 points) The Client should display the board and information if it was a new or running game.</li>
<li>(2 points) The Client should also let the player know in which format the row and column should be entered into the terminal. The error check of input type should be on Client side, the Client will then send the row/column to the server.</li>
<li>(5 points) During the game the Server waits for the Client to send a row and column (in one request). The Server will then check if the values are on the board (so inside the board dimension) and if it was a hit or miss or an already opened tile. The new board and the hit/miss/old info will be sent to the client and should be displayed in a user friendly way. Or of course an error message if out of bounds.</li>
<li>(5 points) Multiple clients can enter the SAME game if one is already in progress and will thus find the ships faster. Make sure that this is thread safe as well.</li>
<li>(5 points) Clients win when finding all ships (always 12 ’x’ on a 7×7 board) and get back to main menu, multiple clients can win together (see video). They will all get 1 point when they are in the game together (no matter if they participated or not) and find all the ships. So basically one win is one point. This will be the “DONE” response.</li>
<li>(3 points) Clients can also lose together, if both Clients together made more than 42 guesses they lose. Yes, this is especially mean since one Client can spam and the other one not do anything about it but just go with it. This is also the DONE response.</li>
<li>(2 points) Give points in some way based on the fewer overall guesses were needed, you can decide on any way you want. Return the points when sending the DONE response on a win.</li>
<li>(2 point) Game quits gracefully when option 3 is chosen in main menu.</li>
<li>(3 points) If user types “exit” while in the game (instead of row or column), the client will exit gracefully after sending a QUIT request to the server and receiving a BYE.</li>
<li>(3 points) Server does not crash when the client just disconnects (without choosing option 3 or exit)</li>
<li>(3 points) Your server/client should not crash even when receiving wrong input and wrong requests/responses. Make sure everything is as robust as possible.</li>
<li>(3 points) You need to run and keep your server running on your AWS instance (or somewhere others can reach it and test it) – if you used the protocol correctly everyone should be able to connect with their Client. You will need to post your exact gradle command we can use (including ip and port) on the #servers channel on Slack. If at least one person commented on your server you can take it offline if you like.</li>
<li>(2 points) You test at least 2 other servers, can be done up to 2 days after the due date. Make a meaningful comment on Slack about it. In case you find an error let the other person know, so they still have a chance to fix it.</li>
</ol>
<strong>NEEDED</strong>: On your server always print the non hidden version of the board, so we can grade faster. Make sure your program is robust with all possible inputs, we should not be able to break it and crash it. We will not be mean when running it but with using it to our best ability and basic “gaming” it should not crash. If we can crash it easily you will loose points for it no matter if the main functionality is there.

<strong>Hints:</strong>

These are some tips you can take them or leave them.

<ul>
<li>Spend some time on the given code, make small changes to it, even if they are stupid. Just to get a feel of Protobuf. Especially with the repeated fields. Get the feel for protobuf before even continuing.</li>
<li>Start with the base functionality, e.g. just test sending one row/col to check for a hit/miss</li>
<li>Setup with threads first and not when the rest is done (I did it the other way and it was more painful to change)</li>
<li>Work incrementally step by step. I usually add one new request with dummy data, check if I receive it on the server. Then add the real data, check if I receive it. Then I parse it on server, check if that works. Then create response and send it to client, check if I receive it. I usually go a couple lines at a time, especially if it is a new concept.</li>
</ul>
<h1>Submission</h1>
On Canvas submit your link to your Assignment 4 folder on GitHub.
