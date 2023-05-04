Download Link: https://assignmentchef.com/product/solved-cs433-homework-1-tweet-analysis-with-mapreduce
<br>












In this homework, you’ll write a MapReduce algorithm to analyze sample twitter dataset containing approximately 3.8 million tweets.




<ul>

 <li>Install Hadoop to your own server or use cs433.cse.unr.edu.</li>

 <li>           You need to use jump host to access cs433.cse.unr.edu from outside of UNR campus. So, you can first login to nxlogin.engr.unr.edu and from there to cs433.cse.unr.edu</li>

 <li>Download ZIP file in here. Its size is around 405 MB. The files are already uploaded to HDFS in cs433.cse.unr.edu under “/” directory. Check by running “Hadoop dfs -ls /homework1/”</li>

 <li>Unzip the file and upload “training_set_tweets.txt” (tweets) and “training_set_users.txt” (users) files to HDFS</li>

</ul>




<u>Once your Hadoop cluster is up and running do the following tasks:</u>

<ul>

 <li>Show HDFS daemons (hint: search for processes called namenode, datanode) <strong>(5 pts)</strong></li>

 <li>Show how many blocks created in HDFS for “tweets” file, either through command line or namenode web ui <strong>(5 pts)</strong></li>

 <li>Show how many map tasks are created when you try to process “tweets” file in HDFS <strong>(10pts)</strong></li>

 <li>Set the number of reduce tasks to 3 and show that Hadoop created 3 reduce tasks  <strong>(10 pts)</strong></li>

 <li>Write a MapReduce code to count the number of hash tags occurrences and find the <u>most repeated 10 hashtags</u>. <strong>(20 pts)</strong></li>

 <li>Write a MapReduce code find the <u>most tweeted 10 days</u>. (Tweets are associated with time stamps so you need to count all the tweets posted in same days) <strong>(20 pts)</strong></li>

 <li>Write a MapReduce code to find the <u>most tweeted 10 cities </u>along with the number of tweets (“training_set_users.txt” file has user_id  city relation to extract city information) <strong>(30 pts)</strong></li>

</ul>

Important Notes

<ul>

 <li>It is <u>NOT</u> allowed to use global variables in Q5 and Q6 as they are easy to implement with single MR job.</li>

 <li>Although it is not an ideal solution, you can use a global variable in Q7 to keep the solution simple. However, I offer <u>10pt</u> bonus points if you implement without using a global variable. You’ll need to write multiple jobs in one application and use reduce-side join to implement this way.</li>

</ul>







What to deliver

Create following files/folders and compress them in <u>a single zip file</u> with name &lt;<strong>LASTNAME&gt;_&lt;NAME&gt;_HW1.zip</strong> and submit on WebCampus




<ul>

 <li>Take screenshots for Question 1-4 to a file <u>answers1-4.pdf</u></li>

 <li>Copy the most repeated 30 hashtags along with number of occurrences to a file called “popular_tweets.txt” file</li>

 <li>Copy the most tweeted 20 days along with number of tweets to a file called “most_tweeted_days.txt” file</li>

 <li>Copy the most tweeted 10 cities along with number of tweets to a file called “most_tweeted_citites.txt” file</li>

 <li>Create three directories Q5, Q6, and Q7 and copy your source code for question 5, 6, and 7 into those directories.</li>

 <li><strong> [Important]</strong> Create <strong>README</strong> file that shows how to run compile and run your code</li>

 <li><strong> [Important] </strong><u>Do not</u> include input files in your final submission</li>

</ul>





