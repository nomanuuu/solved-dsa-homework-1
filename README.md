Download Link: https://assignmentchef.com/product/solved-dsa-homework-1
<br>
<h1>Problem 1 – Complexity</h1>

<strong>Warning: </strong>Conciseness makes everyone’s life easier. You should answer Problem 1 within 3 pages, or you will get some penalties. Also, make sure your answer is clear and easy to read for others.

Suppose that <em>f </em>and <em>g </em>are real-valued functions defined on R<sup>+</sup>, and <em>g</em>(<em>x</em>) is strictly positive for all sufficiently large <em>x </em>(formally, there is some <em>x</em><sub>1 </sub>such that <em>g</em>(<em>x</em>) <em>&gt; </em>0 for all <em>x &gt; x</em><sub>1</sub>). Recall the following asymptotic notations:

<ul>

 <li><em>f</em>(<em>x</em>) = <em>O</em>(<em>g</em>(<em>x</em>)) if and only if there exist positive numbers <em>c </em>and <em>x</em><sub>0 </sub>such that</li>

</ul>

|<em>f</em>(<em>x</em>)| ≤ <em>cg</em>(<em>x</em>) for all <em>x &gt; x</em><sub>0</sub><em>.</em>

<ul>

 <li><em>f</em>(<em>x</em>) = Ω(<em>g</em>(<em>x</em>)) if and only if there exist positive numbers <em>c </em>and <em>x</em><sub>0 </sub>such that</li>

</ul>

|<em>f</em>(<em>x</em>)| ≥ <em>cg</em>(<em>x</em>) for all <em>x &gt; x</em><sub>0</sub><em>.</em>

<ul>

 <li><em>f</em>(<em>x</em>) = Θ(<em>g</em>(<em>x</em>)) if and only if <em>f</em>(<em>x</em>) = <em>O</em>(<em>g</em>(<em>x</em>)) and <em>f</em>(<em>x</em>) = Ω(<em>g</em>(<em>x</em>)).</li>

</ul>

Note that the definitions here may be slightly different to other versions in different textbooks, but they may come in handy in some problems of this section. We ask you to use our definitions here to answer the subproblems below.

Here are some sample tasks and solutions for reference:

<ul>

 <li>The word ”brief” means ”very short”. An example of a <strong>brief </strong>explanation:</li>

</ul>

Sample task: Write down the time complexity for this function using the Θ notation along with an expression of <em>n</em>.

worship-127-double-n(<em>n</em>)

<ul>

 <li><strong>for </strong><em>i </em>= 1<em>..n</em></li>

 <li><strong>for </strong><em>j </em>= 1<em>..</em>2<em>n</em></li>

 <li>print(”Praise 127”)</li>

</ul>

Sample solution 1: The iteration of the loops are <em>n </em>and 2<em>n </em>respectively, so there are 2<em>n</em><sup>2 </sup>iterations. Hence the time complexity is Θ(<em>n</em><sup>2</sup>).

Sample solution 2: 顯然他總共跑 2<em>n</em><sup>2 </sup>次，所以是 Θ(<em>n</em><sup>2</sup>)。

<ul>

 <li>An example of a <strong>formal proof</strong>:</li>

</ul>

<strong>Note: </strong>Recall that <em>f</em>(<em>x</em>) = <em>O</em>(<em>g</em>(<em>x</em>)) if and only if there exist positive numbers <em>c </em>and <em>x</em><sub>0 </sub>such that

|<em>f</em>(<em>x</em>)| ≤ <em>cg</em>(<em>x</em>) for all <em>x &gt; x</em><sub>0</sub><em>.</em>

<strong>If you prove the correctness of a statement S by formal definition, you should specify all constants like </strong><em>c </em><strong>and </strong><em>x</em><sub>0</sub><strong>.</strong>

Sample problem: Prove that <em>an </em>+ <em>b </em>= Θ(<em>n</em>), where <em>a </em>and <em>b </em>are positive constants.

Sample full-credit formal proof 1: Observe that , so

<em>an </em>+ <em>b </em>= Θ(<em>n</em>).

Sample full-credit formal proof 2: Rewrite <em>an </em>+ <em>b </em>= <em>n</em>(<em>a </em>+ <em>bn</em>−<sup>1</sup>). Obviously we have lim<em><sub>n</sub></em>→∞(<em>a </em>+ <em>bn</em>−<sup>1</sup>) = <em>a</em>, so for any fixed <em>ϵ &gt; </em>0, there is some large <em>N </em>such that |<em>a </em>− (<em>a </em>+ <em>bn</em>−<sup>1</sup>)| <em>&lt; ϵ</em>. Take, then for some large <em>N</em>, we have the inequality:

Multiply it by <em>n </em>we have

so <em>an </em>+ <em>b </em>= Θ(<em>n</em>).

Sample full-credit formal proof 3: Obviously <em>an </em>= <em>O</em>(<em>n</em>) and <em>b </em>= <em>O</em>(<em>n</em>), by the theorem 併吞律 we have <em>an </em>+ <em>b </em>= <em>O</em>(<em>n</em>).

Now, imagine that you are on the magic train heading to the empire of God 127, the master of algorithm. To worship God 127, you should have some skills to evaluate the complexity of simple function calls.

Read the following pseudo code carefully. Write down the time complexity for each of the following function using the Θ notation along with an expression of <em>n</em>. <strong>Your answer should be as simple as possible. </strong>For instance,  should be written as Θ(<em>n</em><sup>2</sup>).

Your answer should also come with a <strong>brief </strong>explanation.

<ol>

 <li>(5 pts)</li>

</ol>

func-a(<em>n</em>)

<ul>

 <li><em>sum </em>= 0<em>,i </em>= 1</li>

 <li><strong>while </strong><em>sum </em><em>&lt; n</em></li>

 <li><em>sum </em>= <em>sum </em>+ <em>i</em></li>

 <li><em>i </em>= <em>i </em>+ 1</li>

</ul>

<ol start="2">

 <li>(5 pts)</li>

</ol>

func-b(<em>n</em>)

<ul>

 <li><em>m </em>= 2</li>

 <li><strong>while </strong><em>m &lt; n</em></li>

 <li><em>m </em>= <em>m </em>∗ <em>m</em></li>

</ul>

<ol start="3">

 <li>(10 pts)</li>

</ol>

func-c(<em>n</em>)

<ul>

 <li><strong>if </strong><em>n &gt; </em>87506055</li>

 <li>func-c(<em>n </em>− 1)</li>

 <li>func-c(<em>n </em>− 1)</li>

 <li>func-c(<em>n </em>− 1)</li>

 <li>func-c(<em>n </em>− 1)</li>

 <li><strong>elseif </strong><em>n &gt; </em>0</li>

 <li>func-c(<em>n </em>− 1)</li>

 <li>func-c(<em>n </em>− 1)</li>

 <li>func-c(<em>n </em>− 1)</li>

</ul>

Finally, you arrives at the entrance of 127’s empire. However, the soldiers won’t let you pass the entrance if you are not familiar with asymptotic notations. For the next six subproblems, consider <em>n </em>to be a positive integer and <em>f</em>(<em>n</em>)<em>,g</em>(<em>n</em>)<em>,i</em>(<em>n</em>)<em>,j</em>(<em>n</em>) to be <em>positive</em>, <em>monotonically increasing </em>functions with <em>non-negative </em>domains.<a href="#_ftn1" name="_ftnref1"><sup>[1]</sup></a> Prove or disprove each of the statement. You should provide a <strong>formal proof </strong>if you believe the statement to be true, or a counterexample if you believe the statement to be false.

<ol start="4">

 <li>(10 pts) (Prove or disprove) <em>f</em>(<em>n</em>) + <em>g</em>(<em>n</em>) = Θ(max(<em>f</em>(<em>n</em>)<em>,g</em>(<em>n</em>))).</li>

 <li>(10 pts) (Prove or disprove) If <em>f</em>(<em>n</em>) = <em>O i</em>(<em>n</em>) and <em>g</em>(<em>n</em>) = <em>O j</em>(<em>n</em>) , then <em>f</em>(<em>n</em>) · <em>g</em>(<em>n</em>) =</li>

</ol>

<em>O</em>(<em>i</em>(<em>n</em>) · <em>j</em>(<em>n</em>)).                                               (       )             <em>f</em>(<em>n</em>)             ( <em>g</em>(<em>n</em>))

(        )                            (        )

<ol start="6">

 <li>(10 pts) (Prove or disprove) If <em>f</em>(<em>n</em>) = <em>O g</em>(<em>n</em>) , then 2 = <em>O </em>2 .</li>

</ol>

Did you have fun warming up? Now the soldiers are giving you more challenging ones. Try your best! Some calculus tricks may help. We encourage you to use results from the lecture slides to make your proof shorter.

<ol start="7">

 <li>(10 pts) (Prove or disprove) The harmonic series.</li>

 <li>(10 pts) (Prove or disprove) lg(<em>n</em>!) = Θ(<em>n</em>lg<em>n</em>).</li>

</ol>

Finally, you get to meet God 127 face to face. He decides to give you the final trial with a recursive function to test if you are able to pass this course. &#x1f609;

<ol start="9">

 <li>(10 pts) Define</li>

</ol>

1<em>,                             </em>if <em>n </em>= 1

<em>f</em>(<em>n</em>) =

otherwise

Please find the tightest bound of <em>f</em>(<em>n</em>) with Θ notation. You should provide a proof to get credits. Answers without any proof will receive NO credits.

Congratulations on completing all the proof—<em>or not? </em>Those mathematically inclined can try two more subproblems below. Those subproblems are harder and do not carry many points, but tackling them surely gives you some self-satisfaction!

<ol start="10">

 <li>(Bonus 10 pts) (Prove or disprove) be a sequence of real-valued functions defined on R<sup>+ </sup>such that <em>f<sub>k</sub></em>(<em>n</em>) = <em>O</em>(<em>n</em><sup>2</sup>) for <em>k </em>∈ N, then.</li>

 <li>(Bonus 10 pts) The following pseudo code is the famous Euclidean algorithm for computing the greatest common divisor—hmm, where have you seen this task? &#x1f609;</li>

</ol>

euclidean-gcd(<em>m,n</em>)

<ul>

 <li><strong>while </strong><em>m </em>= 0̸</li>

 <li>(<em>m,n</em>) = (<em>n </em>mod <em>m,m</em>) 3 <strong>return </strong><em>n</em></li>

</ul>

Please show that the worst time complexity for this algorithm is <em>O</em>(lg(<em>m </em>+ <em>n</em>)).

<h1>Problem 2 – Stack / Queue</h1>

@

First, please design an algorithm that reverses the content of a <em>source </em>queue using an additional <em>helper </em>queue that is initially empty. For example, consider a source queue originally contains [1,2,3], where 3 is at the front of the queue. After running the algorithm, the source queue should become [3,2,1], where 1 is at the front, with the helper queue empty. The algorithm can only use <em>O</em>(1)-extra space in addition to the two queues. You have to guarantee that the algorithm runs in <em>O</em>(<em>n</em><sup>2</sup>)-time where <em>n </em>is the number of elements in the queue. In addition to the usual <em>enqueue,dequeue, </em>and <em>front </em>of the queue, you may assume that the queues above also supports <em>size</em>, which returns the current number of elements in the queue.

<ol>

 <li>(10 pts) Show your algorithm with any pseudo code.</li>

 <li>(10 pts) Prove that your algorithm in the previous subproblem runs in <em>O</em>(<em>n</em><sup>2</sup>)-time.</li>

</ol>

Next, let’s play with another data structure. Whereas a stack allows insertion and deletion of elements at only one end, and a queue allows insertion at one end and deletion at the other end, a <em>deque </em>(double-ended queue) allows insertion and deletion at both ends. Please use any pseudo code to implement a deque by using two stacks and at most <em>O</em>(1)-extra space, and answer the following five subproblems. A deque should support four operations, as listed below. You can assume that there is no invalid operation like popping from an empty deque.

<ol start="3">

 <li>(10 pts) Illustrate your design, in particular, how you achieve each of the four operations below (preferably with figures).</li>

</ol>

Then, briefly describe the time complexity of each operation under your design—the faster the better.

<ol start="4">

 <li>(5 pts) void push_front(int x): Insert an element to the front end of the deque.</li>

 <li>(5 pts) void push_back(int x): Insert an element to the back end of the deque.</li>

 <li>(5 pts) int pop_front(): Remove and return the element at the front end of the deque.</li>

 <li>(5 pts) int pop_back(): Remove and return the element at the back end of the deque.</li>

</ol>

Finally, let’s have more fun with the stack. Arguably the simplest way to implement a stack is to use a consecutive array and push to the “end” of the consecutive region. However, the arraybased one is limited by the allocated capacity of the underlying array. One way to conquer the limitation is to dynamically enlarge the array when it is full, which is commonly called a dynamic-array implementation.

<ol start="8">

 <li>(10 pts) Consider the following dynamic-array implementation of a stack; please analyze the time needed for n consecutive push operations. You can assume that each realloc operation takes <em>O</em>(<em>m</em>)-time where <em>m </em>is the number of elements in the array.</li>

</ol>

struct Stack { int top; int capacity; int *arr;

}

struct Stack *createStack() { struct Stack *S = malloc(sizeof(struct Stack));

S-&gt;capacity = 1;

S-&gt;top = -1;

S-&gt;arr = (int*)malloc(S-&gt;capacity * sizeof(int)); return S;

}

int isFullStack(struct Stack *S) { return (S-&gt;top == S-&gt;capacity-1);

}

void enlarge(struct Stack *S) { int new_capacity = (S-&gt;capacity * 3);

S-&gt;capacity = new_capacity;

S-&gt;arr = (int*)realloc(S-&gt;arr, new_capacity * sizeof(int));

}

void push(struct Stack *S, int data) { S-&gt;arr[++S-&gt;top] = data; if (isFullStack(S)) enlarge(S);

}

<h1>Problem 3 – Array / Linked Lists</h1>

For all subproblems below, your answers should include the following parts:

<ul>

 <li>Describe the workflow of your algorithm and briefly explain why it works.</li>

 <li>Analyze the time complexity and extra-space complexity of your algorithm. If your algorithm is not efficient enough in time or in space, you may not get full points.</li>

</ul>

First, consider a read-only array <em>A </em>that contains <em>n </em>integers ∈ {0<em>,</em>1<em>,…,n</em>−1}, where “readonly” means that you cannot modify the contents of the array. A frog, starting from some legitimate initial position within <em>A</em>, jumps within <em>A</em>[0]<em>,A</em>[1]<em>,…,A</em>[<em>n</em>−1] by the following rule.

<ul>

 <li>If the frog is on the <em>i<sup>th </sup></em>position and <em>A</em>[<em>i</em>] ≠ <em>i</em>, it will jump to the (<em>A</em>[<em>i</em>])<em><sup>th </sup></em></li>

 <li>If the frog is on the <em>i<sup>th </sup></em>position and <em>A</em>[<em>i</em>] = <em>i</em>, it will stop.</li>

</ul>

<ol>

 <li>(15 pts) Given the initial position of the frog, design an algorithm that computes whether the frog will stop somewhere or keep jumping forever.</li>

 <li>(15 pts) Given an <em>A </em>such that <em>A</em>[<em>i</em>] ≠ <em>i, </em>∀<em>i </em>0 ≤ <em>i &lt; n</em>, which means that the frog is doomed to keep jumping forever from any initial position. Then, the frog will eventually jump into a “loop” of indices. Given the initial position of the frog, design an algorithm that computes the length of the loop.</li>

</ol>

For example, <em>A </em>= [1<em>,</em>0<em>,</em>4<em>,</em>2<em>,</em>3<em>,</em>1<em>,</em>4<em>,</em>6].

<ul>

 <li>When the initial position is on 0, 1, or 5, the frog jumps into the loop 0 → 1 → 0 → 1···. The length of the loop is 2.</li>

 <li>When the initial position is on 2, 3, 4, 6, or 7, the frog jumps into the loop 2 → 4 → 3 → 2 → 4 → 3···. The length of the loop is 3.</li>

</ul>

Enough with the frog. The next subproblem is about the sorted array.

<ol start="3">

 <li>(15 pts) <em>A </em>is a strictly increasing array with <em>n </em>integers, where <em>A </em>= [<em>a</em><sub>0</sub><em>,a</em><sub>1</sub><em>,</em>·· <em>,a<sub>n</sub></em>−2<em>,a<sub>n</sub></em>−1], <em>n </em>≥ 3. Now, consider the following definitions.

  <ul>

   <li><em>A<sub>s,t </sub></em>= [<em>a<sub>s</sub>,a<sub>s</sub></em><sub>+1</sub><em>,</em>·· <em>,a<sub>t</sub></em>−2<em>,a<sub>t</sub></em>−1], where 0 ≤ <em>s &lt; t </em>≤ <em>n</em></li>

   <li><em>M<sub>s,t </sub></em>= the median of <em>A<sub>s,t</sub></em></li>

   <li><em>f</em>(<em>i,j</em>) = max(<em>M</em><sub>0<em>,i</em></sub><em>,M<sub>i,j</sub>,M<sub>j,n</sub></em>) − min(<em>M</em><sub>0<em>,i</em></sub><em>,M<sub>i,j</sub>,M<sub>j,n</sub></em>), where 0 <em>&lt; i &lt; j &lt; n</em></li>

  </ul></li>

</ol>

In short, <em>A </em>is partitioned into three subarrays by index <em>i </em>and index <em>j</em>. Each subarray has its own median. <em>f</em>(<em>i,j</em>) equals to ”the maximum of three medians” minus ”the minimum of three medians”.

Design an algorithm to find a pair (<em>i,j</em>), where 0 <em>&lt; i &lt; j &lt; n</em>, such that <em>f</em>(<em>i,j</em>) is minimized.

Finally, let’s play with a new kind of linked list.

<ol start="4">

 <li>(15 pts) A circularly linked list is a linked list such that the last node of the linked list is connected to the head instead of some nil (NULL) value. We call a node <em>A </em>decreasing in the circularly linked list if <em>next.value &lt; A.value</em>.</li>

</ol>

Consider a circularly linked list <em>L </em>with <em>n </em>integers, represented by some head node. Assume that there are two decreasing nodes within <em>L</em>. Design an algorithm that “sorts” all nodes within <em>L </em>such that head points to a new circularly linked list with only one decreasing node. We expect the algorithm to run in <em>O</em>(<em>n</em>)-time and <em>O</em>(1)-extra-space .

<strong> Programming Part </strong>

<h1>Problem 4 – Evil Eval</h1>

<h2>Problem Description</h2>

In this problem, you “simply” have to implement a calculator like what has been taught in the classes. The calculator should support the following operator on double-precision floating points with correct precedence:

<ul>

 <li>arithmetic operators: +<em>, </em>–<em>, </em>*<em>, </em>/</li>

 <li>parentheses: (<em>, </em>)</li>

</ul>

It is guaranteed that the divisor would not be zero during the process of the calculation.

Please do not try to solve this problem by calling other program in your source code. If (and only if) you patiently, wholeheartedly code the homework out, you will gain a better coding skill and a deeper understanding of the data structure!

<strong>Input</strong>

The input contains <em>T </em>lines, each representing an arithmetic expression.

<h2>Output</h2>

For each test case print a double-precision floating point number in one line, which indicates the answer of the expression. Your solution will be considered correct if the absolute or relative error between the answer and your output is less than 10−<sup>12</sup>. Formally, let your answer be <em>a</em>, and the jury’s answer be <em>b</em>, your answer is accepted if and only if

<h2>Constraints</h2>

<ul>

 <li>0 &lt; the length of each line <em>L </em>&lt; 10<sup>6</sup></li>

 <li>0 <em>&lt; a<sub>i </sub>&lt; </em>10<sup>8 </sup>for each number <em>a<sub>i </sub></em>in the expression</li>

 <li><em>L </em> <em>T </em>≤ 10<sup>6</sup></li>

 <li>every numbers in the input will be an integer containing only of digits. We expect the final output to be a floating point number, though.</li>

</ul>

<strong>Subtask 1 (25 pts)</strong>

<ul>

 <li>the operator include only +, –</li>

</ul>

<strong>Subtask 2 (25 pts)</strong>

<ul>

 <li>the operators include only +, -, *, /</li>

</ul>

<strong>Subtask 3 (50 pts)</strong>

<ul>

 <li>all operators are possible</li>

</ul>

<h1>Sample Cases</h1>

<strong>Sample Input 1</strong>

1+3-2

<strong>Sample Output 1</strong>

2.000000000000000

<h2>Sample Input 2</h2>

1+2*3

1-2*3

<h2>Sample Output 2</h2>

7.000000000000000

-5.000000000000000

<strong>Sample Input 3</strong>

(1+2)*3

<strong>Sample Output 3</strong>

9.000000000000000

<h1>Problem 5 – Waston and Abili</h1>

<h2>Problem Description</h2>

Waston and Abili runs a consulting detective service. In a recent case, a train storage station of British Railway drew their attention. They suspect that the operator of the station hid something illegal in the train storage station by manipulating the records. To check if there is any mismatch with the official record, they sneaked into the station and have only one night to find out which train cabin is not recorded.

As their friend and one who has extreme self-confidence in programming, you want to write a program that reads in the parking logs and print out a map of the storage station. The log begins with two integers, <em>k</em>, <em>n</em>, denoting the mount of parking rails and the records in the log respectively.

There are three types of logs in the official record.

<ol>

 <li>Cabin with label <em>l </em>enters the <em>r</em>-th rail</li>

</ol>

In this station, <strong>each parking rail has only one entrance, which is also the exit</strong>, so only the last cabin that entered the rail can leave the rail. If a cabin with label <em>l </em>entered the <em>r</em>-th parking rail, the corresponding log will be enter r l

<ol start="2">

 <li>The last cabin stored in the <em>r</em>-th rail leaves that rail</li>

</ol>

If the last cabin of <em>r</em>-th rail leaves the station, the corresponding log will be leave r

<ol start="3">

 <li>The <em>r<sub>a</sub></em>-th rail is shut down for maintenance, all the cabins is migrated to the <em>r<sub>b</sub></em>-th rail one by one.</li>

</ol>

Sometimes, the operator shutdowns certain rails for railway maintenance. In such scenario, all cabins of the maintenance rail leaves and enters another one by one. If the <em>r<sub>a</sub></em>-th rail is shut down, and all its cabins is migrated into the <em>r<sub>b</sub></em>-th cabin, then the corresponding log will be migrate r_a r_b

There might be some mistakes in the logs, for example, a cabin leaving from an empty rail. In such case, just ignore all the illegal logs. After processing all logs, please output what the cabin arrangement should be like in the station from the 0-th rail to (<em>k </em>− 1)-th rail.

Below is an illustration of a station with 3 rails and 6 cabins.

<h1>Input Format</h1>

The first line contains two integer <em>k,n</em>. The next <em>n </em>lines may be in below three formats:

<ol>

 <li>enter follow by two integer <em>r</em>, <em>l</em></li>

 <li>leave follow by one integer <em>r</em></li>

 <li>migrate follow by two integer <em>r<sub>a</sub>,r<sub>b</sub></em></li>

</ol>

<h1>Output Format</h1>

You should output <em>k </em>lines, each containing the labels of train cabins parked in each rail by the order they entered the rail. For example, the <em>i</em>-th line contains the labels of cabins parked in rail <em>i</em>.

<h1>Constraint</h1>

<ol>

 <li>1 ≤ <em>n </em>≤ 10<sup>6</sup></li>

 <li>2 ≤ <em>k </em>≤ 10<sup>3</sup></li>

 <li>0 ≤ <em>r,r<sub>a</sub>,r<sub>b </sub>&lt; k,r<sub>a </sub></em>≠ <em>r<sub>b</sub></em></li>

 <li>0 ≤ <em>l </em>≤ 10<sup>4</sup>, noted that <em>l </em>is not necessarily unique</li>

</ol>

<h2>Subtasks</h2>

<strong>Subtask 1 (25 pts)</strong>

<ul>

 <li>1 ≤ <em>n </em>≤ 10<sup>3</sup></li>

 <li>1 ≤ <em>k </em>≤ 10</li>

 <li>No migrate operation</li>

</ul>

<strong>Subtask 2 (50 pts)</strong>

<ul>

 <li>1 ≤ <em>n </em>≤ 10<sup>4</sup></li>

 <li>10 ≤ <em>k</em></li>

</ul>

<strong>Subtask 3 (25 pts)</strong>

<ul>

 <li>No ⊕ther constraints!</li>

 <li>You might want to search for “how to reverse a linked list in less than <em>O</em>(<em>n</em>) time” to solve this problem</li>

 <li>GL &amp; HF &#x1f61b;</li>

</ul>

<h1>Sample Cases</h1>

<table width="490">

 <tbody>

  <tr>

   <td width="328"><strong>Sample Input 1</strong>3 7 enter 1 1</td>

   <td width="162"><strong>Sample Output 1</strong>1 2 4 3</td>

  </tr>

 </tbody>

</table>

enter 1 2 enter 2 3 enter 2 4 enter 2 5 leave 2 migrate 2 1

Note that there are two empty lines , one above and the other below 1 2 4 3. For more sample cases, go to the problem page on DSA Judge.

<h1>Problem 6 – K-Least Element in the Sequence</h1>

<h2>Problem Description</h2>

Giver is a beginner at programming, so he practices hard everyday for improving his skill. One day, someone asks him a problem: “Given a sequence <em>a</em><sub>1</sub><em>,a</em><sub>2</sub><em>,…,a<sub>n</sub></em>, please find the <em>k</em>-least element in the sequence.” However, Giver is so clever that this problem is too easy for him. Therefore, He tries to modify the problem to make it harder. Now, the problem becomes as follows:

Given a sequence <em>a</em><sub>1</sub><em>,a</em><sub>2</sub><em>,…,a<sub>n</sub></em>, you are asked to support the following operations.

<ul>

 <li>Insert <em>i x </em>– insert an integer <em>x </em>before the <em>i</em>th element of the sequence. If <em>i </em>− 1 equals the length of the sequence, then insert <em>x </em>at the end of it.</li>

 <li>Delete <em>i </em>– delete the <em>i</em>th element of the sequence.</li>

 <li>Reverse <em>l r </em>– reverse the elements between the interval [<em>l,r</em>] of the sequence.</li>

 <li>Query <em>l r k </em>– find the <em>k</em>-least element between the interval [<em>l,r</em>] of the sequence.</li>

</ul>

<h2>Input</h2>

The first line contains two integers <em>n,q </em>(1 ≤ <em>n,q </em>≤ 50000), representing the length of the initial sequence and the number of operations respectively. The second line contains the initial sequence, which consists of <em>n </em>integers <em>a</em><sub>1</sub><em>,a</em><sub>2</sub><em>,…,a<sub>n </sub></em>(−10<sup>5 </sup>≤ <em>a</em><sub>1</sub><em>,a</em><sub>2</sub><em>,…,a<sub>n </sub></em>≤ 10<sup>5</sup>).

Each of the next <em>q </em>lines is an operation with the format mentioned above.

It is guaranteed that all operations are valid. Formally, suppose that the current length of the sequence is <em>N</em>, then it must satisfy the following constraints.

<ul>

 <li>Insert <em>i x</em>: 1 ≤ <em>i </em>≤ <em>N </em>+ 1<em>, </em>−10<sup>5 </sup>≤ <em>x </em>≤ 10<sup>5</sup>.</li>

 <li>Delete <em>i</em>: 1 ≤ <em>i </em>≤ <em>N</em>.</li>

 <li>Reverse <em>l r</em>: 1 ≤ <em>l </em>≤ <em>r </em>≤ <em>N</em>.</li>

 <li>Query <em>l r k</em>: 1 ≤ <em>l </em>≤ <em>r </em>≤ <em>N, </em>1 ≤ <em>k </em>≤ <em>r </em>− <em>l </em>+ 1.</li>

</ul>

<h2>Output</h2>

For each ”Query <em>l r k</em>” operation, print an integer, representing the <em>k</em>-least integer between the <em>l</em>th element and the <em>r</em>th element.

<strong>Subtask 1 (20 pts)                                                      Subtask 3 (5 pts)</strong>

<ul>

 <li><em>n,q </em>≤ 3000. There are only “Insert”, “Delete”, “Re-</li>

</ul>

verse” operations.

<strong>Subtask 2 (25 pts)                                                      Subtask 4 (50 %)</strong>

<ul>

 <li>There are only “Query” operations. No other constraints.</li>

</ul>

<h2>Sample Input 1                                        Sample Output 1</h2>

5 5                                -3

-10 1 4 -3 -5                      -10

Query 4 4 1                        -3

Query 1 2 1                        4

Query 4 5 2                        -5

Query 2 3 2

Query 4 5 1

<h2>Sample Input 2                                        Sample Output 2</h2>

5 5                                4

-2 4 4 -7 2                        -7

Delete 5

Delete 1

Insert 2 6

Query 3 3 1

Query 4 4 1

<h2>Sample Input 3                                        Sample Output 3</h2>

5 5                                -6

-6 7 3 3 0                         -6

Reverse 1 4 Insert 3 -6

Query 3 4 1

Reverse 4 5

Query 1 4 2

<h2>Hints</h2>

<ol>

 <li>You may need the data structure like linked list to support efficient modification.

  <ul>

   <li>Due to the bad performance on interval operation and indexing, you may want to reduce the number of nodes.</li>

   <li>Try to bind some elements into one node, that is, store a sequence of elements using an sequence in a node.</li>

   <li>Try to maintain the nodes such that both the number of nodes and the number of elements in a node are not too big. That is, you may need to split a node or rebuild the data structure if one of them is too large.</li>

  </ul></li>

 <li>How to reverse a segment that can be represented by a sequence of nodes? what if not, can you make it become the same case? You may need to add a tag on each node and reverse it some time later to preserve a good time complexity.</li>

 <li>You may need to use the binary search algorithm when finding the <em>k</em>-least element. You may also need to maintain some more information for each node to support efficient query.</li>

</ol>

<a href="#_ftnref1" name="_ftn1">[1]</a> A function <em>f </em>is monotonically increasing if for all <em>n</em><sub>1</sub>, <em>n</em><sub>2 </sub>such that <em>n</em><sub>1 </sub><em>&lt;n</em><sub>2</sub>, we have <em>f</em>(<em>n</em><sub>1</sub>) ≤<em>f</em>(<em>n</em><sub>2</sub>).