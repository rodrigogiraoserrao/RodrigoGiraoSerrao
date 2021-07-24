**Hey there, I'm Rodrigo** 👋


## A little bit about myself

- 🔭 I’m currently working on my personal project: [mathspp.com](https://mathspp.com)
- 💬 Ask me about mathematics, programming and bad jokes.
- 📫 You can find my contacts [here](https://mathspp.com/about#contacts).
- 😄 Pronouns: he/him/his


## 📖 My most recent articles

<!-- BLOG-POST-LIST:START -->- [Code style matters | Pydon't](https://mathspp.com/blog/pydonts/code-style-matters) (Mon Jul 19 2021 10:00 PM)

 > 
                
                                <img alt="" src="https://mathspp.com/images/0/3/9/b/1/039b1565d1a93bd14d152fc7cd6fdfe8bd21bfdc-thumbnail.png" />
                                <p>In this Pydon't I talk about Python style and I go over some tools you can use to help you remain within a consistent style.</p>

<p><img alt="A badly formatted Python function" src="/user/pages/02.blog/04.pydonts/code-style-matters/thumbnail.png"></p>
<p>(If you are new here and have no idea what a Pydon't is, you may want to read the
<a href="/blog/pydonts/pydont-manifesto">Pydon't Manifesto</a>.)</p>
<h1>Introduction</h1>
<p>The overall style of your code can have a great impact
on the readability of your code.
And code is more often read than written,
so you (and others!) have a lot to benefit from you writing
well stylised code.</p>
<p>In this Pydon't, you will:</p>
<ul><li>understand the importance of having a consistent style; and</li>
<li>learn about tools that help you with your code style.</li>
</ul><p>By the way, this week I wrote a shorter and lighter article,
as I am still investing lots of time <a href="https://ep2021.europython.eu/profiles/rodrigo-girao-serrao/">preparing for
Euro Python 2021</a>...
I hope you still find it useful!</p>
<!--v-->
<blockquote>
<p>You can now get your copy of the ebook &ldquo;Pydon'ts &ndash; Write beautiful Python code&rdquo; <a href="https://gum.co/pydonts" target="_blank" rel="nofollow noopener noreferrer" class="external-link no-image">on Gumroad</a>
to help support the series of &ldquo;Pydon't&rdquo; articles &#128170;.</p>
<!--^-->
</blockquote>
<h1>Code style</h1>
<h2>Consistency</h2>
<p>Humans are creatures of habit.
From the fact that the first leg that goes into your trousers is always the same,
to the fact that you always start brushing your teeth on the same side.</p>
<p>These habits automate routines that do not require much attention,
so that you can spend your precious brain power on other things.</p>
<p>As far as my experience goes, the same can be said about your coding style:
if you write with a consistent code style,
it becomes easier to read because you already expect a given structure;
you are only left with acquiring the information within that structure.</p>
<p>Otherwise, if your style isn't consistent,
you have to spend more precious brain power parsing the structure of what you are reading
and only then apprehend the information within that structure.</p>
<p><a href="https://www.python.org/dev/peps/pep-0008/" target="_blank" rel="nofollow noopener noreferrer" class="external-link no-image">PEP 8</a> is a document whose purpose is to outline a style guide
for those who write Python code.
It has plenty of useful recommendations.
However, right after the introduction, PEP 8 reads</p>
<blockquote>
<p>&ldquo;A style guide is about consistency.
Consistency with this style guide is important.
Consistency within a project is more important.
Consistency within one module or function is the most important.</p>
<p>However, know when to be inconsistent -- sometimes style guide recommendations just aren't applicable.
When in doubt, use your best judgment.
Look at other examples and decide what looks best.
And don't hesitate to ask!&rdquo;</p>
</blockquote>
<p>This is very important: PEP 8 is a style guide that contains <em>recommendations</em>,
not laws or strict rules.
And what is more, notice that there is a strong focus on <em>consistency</em>.
Using your own (possibly weird) style consistently is better than using no style at all.
That's if you are working alone; in a project, it is a good idea to decide on
a particular style beforehand.</p>
<h2>Whitespace matters</h2>
<p>When I'm teaching Python, I often do some sort of live coding,
where I explain things and type examples,
that I often ask...</p>
                
            - [Bite-sized refactoring | Pydon't](https://mathspp.com/blog/pydonts/bite-sized-refactoring) (Mon Jul 12 2021 10:00 PM)

 > 
                
                                <img alt="" src="https://mathspp.com/images/2/9/a/b/a/29aba3b57cd3b3d1b9753d595c2a997a073c9cf5-thumbnail.png" />
                                <p>In this Pydon't I show you why refactoring is important
and show you how to do it in little steps,
so that it doesn't become too overwhelming.</p>

<p><img alt="An abstract background with the Python logo and three arrows in a circle, alluding to the 'recycle' symbol." src="/images/5/3/f/6/b/53f6bdd62c2bade7027ab855949f264d5fbd94a1-thumbnail.png"></p>
<p>(If you are new here and have no idea what a Pydon't is, you may want to read the
<a href="/blog/pydonts/pydont-manifesto">Pydon't Manifesto</a>.)</p>
<h1>Introduction</h1>
<p>Refactoring code is the act of going through your code and
changing bits and pieces, generally with the objective of
making your code shorter, faster, or better any metric you set.</p>
<p>In this Pydon't I share my thoughts on the importance of refactoring
and I share some tips for when you need to refactor your code,
as I walk you through a refactoring example.</p>
<p>In this Pydon't, you will:</p>
<ul><li>understand the importance of refactoring;</li>
<li>walk through a real refactoring example with me; and</li>
<li>learn tips to employ when refactoring your own code.</li>
</ul><!--v--><blockquote>
<p>You can now get your copy of the ebook &ldquo;Pydon'ts &ndash; Write beautiful Python code&rdquo; <a href="https://gum.co/pydonts" target="_blank" rel="nofollow noopener noreferrer" class="external-link no-image">on Gumroad</a>
to help support the series of &ldquo;Pydon't&rdquo; articles &#128170;.</p>
<!--^-->
</blockquote>
<h1>Refactoring</h1>
<blockquote>
<p>REFACTOR &ndash; verb</p>
<p>&ldquo;restructure (the source code of an application or piece of software) so as to improve operation without altering functionality.&rdquo;</p>
</blockquote>
<p>As you can see from the definition above,
the act of refactoring your code is an attempt at making your code better.
Making your code better might mean different things,
depending on your context:</p>
<ul><li>it might mean it is easier to maintain;</li>
<li>it might mean it is easier to explain to beginners;</li>
<li>it might mean it is faster;</li>
<li>...</li>
</ul><p>Regardless of the metric(s) you choose to improve,
everyone can benefit from learning to refactor code.</p>
<p>Why is that?</p>
<p>When you are refactoring code you are training a series of skills
that are helpful to you as a developer, like your ability to read
code and really comprehend it, pattern recognition skills,
critical thinking, amongst others.</p>
<h2>Ability to read code and really comprehend it</h2>
<p>If you change a piece of code without understanding it,
you are much more likely to break it.
Therefore, when you want to refactor a piece of code,
you should do your best to try and <em>really</em> comprehend what the code
is doing and how it does it.</p>
<h2>Pattern recognition skills</h2>
<p>One of the things that you should be looking out for,
when refactoring code,
is redundancies and repetitions.
If you see code that looks like it was copied and pasted,
or if you find code that has a very similar structure,
then it probably is a good target for refactoring.</p>
<p>Sometimes, spotting these things is very simple,
because there will be lines of code that are <em>identical</em>.
However, finding <em>structural</em> similarities between
different parts of your code is harder than finding identical lines,
so in trying to spot these you will be training your pattern
recognition skills.
Beware that this becomes much easier to do <em>after</em>
you have really understood the code.</p>
<h2>Critical thinking</h2>
<p>When reading code you wish to refactor,
you will invariably find pieces of code that look like they shouldn't
be...</p>
                
            - [Problem #040 – the dozen puzzle](https://mathspp.com/blog/problems/the-dozen-puzzle) (Sat Jul 10 2021 10:00 PM)

 > 
                
                                <img alt="" src="https://mathspp.com/images/8/a/0/2/4/8a024e2c2092256def177e595e0997f9aebeae33-thumbnail.png" />
                                <p>Three friends are given three different numbers that add up to a dozen.
Can you figure out everyone's numbers?</p>

<figure class="image-caption"><img title="Photo by Kelly Neil on Unsplash" alt="" src="/images/a/a/0/b/2/aa0b240274949f66f7e54b1af3d29a0785bb9771-thumbnail.png"><figcaption class="">Photo by Kelly Neil on Unsplash</figcaption></figure>
<h1>Problem statement</h1>
<p>Three friends, Alice, Bob, and Charlie, are assigned three different
positive whole numbers by their fourth friend, Diane.
Furthermore, Diane told them that their three numbers add up to 12
and that Charlie's is the largest one.</p>
<p>Diane then asks the three of them if they know everyone's numbers,
to which Bob replies “I do!”, whereas Alice and Charlie remain silent.
After Bob's revelation, Alice and Charlie think for a couple of seconds
and confirm that now they also know everyone's numbers.</p>
<p>What were Alice's, Bob's, and Charlie's numbers?</p>
<div class="notices blue">
<p>Give it some thought!</p>
</div>
<p>If you need any clarification whatsoever, feel free to ask in the comment section below.</p>
<h1>Solvers</h1>
<p>Congratulations to the ones that solved this problem correctly and, in particular, to the ones
who sent me their correct solutions:</p>
<ul>
<li>Ashok M., India;</li>
<li>David H., Taiwan;</li>
<li>Attila K., Hungary;</li>
<li>Jason P., US;</li>
<li>“Starsmer”, US;</li>
</ul>
<p>Join the list of solvers by <a href="mailto:rodrigo@mathspp.com?subject=Solution%20to%20Problem%20#040%20%E2%80%93%20the%20dozen%20puzzle" class="mailto">emailing me</a> your solution!</p>
<h1>Solution</h1>
<p>The solution to this problem will be posted here after this problem has been live for 2 weeks.</p>
<p>This problem was taken from <a href="https://www.reddit.com/r/puzzles/comments/o62ddq/dozen_total_puzzle/" target="_blank" rel="nofollow noopener noreferrer" class="external-link no-image">this Reddit post</a>,
and shared with permission.</p>
<!-- v -->
<p><a href="https://mathspp.com/subscribe">Don't forget to subscribe to the newsletter</a> to get bi-weekly
problems sent straight to your inbox and to add your reaction below.</p>
<!-- ^ -->
                
            - [Does elegance matter? | Pydon't](https://mathspp.com/blog/pydonts/does-elegance-matter) (Mon Jul 05 2021 10:00 PM)

 > 
                
                                <img alt="" src="https://mathspp.com/images/3/2/0/c/3/320c3e055ddc93f4bac395fcff504c15ee16e2d7-thumbnail.png" />
                                <p>Does elegance matter when writing computer programs..?</p>

<p><img alt='"Elegance is not a dispensable luxury, but a crucial matter that decides between success and failure.", quote by Edsger W. Dijkstra.' src="/user/pages/02.blog/04.pydonts/does-elegance-matter/thumbnail.svg"></p>
<p>(If you are new here and have no idea what a Pydon't is, you may want to read the
<a href="/blog/pydonts/pydont-manifesto">Pydon't Manifesto</a>.)</p>
<h1>Introduction</h1>
<p>At the time of writing this article, I am finishing the preparation
of <a href="https://ep2021.europython.eu/talks/Bz5dtEe-pydonts/" target="_blank" rel="nofollow noopener noreferrer" class="external-link no-image">my Python conference talk &ldquo;Pydon'ts&rdquo;</a> at <a href="https://ep2021.europython.eu/" target="_blank" rel="nofollow noopener noreferrer" class="external-link no-image">EuroPython</a>.</p>
<p>For that matter, today's Pydon't will be a bit different.
Usually, I write about using Python's core features to write idiomatic, expressive,
elegant Python code.
In this Pydon't I will share with you <em>why</em> this is important.</p>
<!--v-->
<blockquote>
<p>You can now get your copy of the ebook &ldquo;Pydon'ts &ndash; Write elegant Python code&rdquo; <a href="https://gum.co/pydonts" target="_blank" rel="nofollow noopener noreferrer" class="external-link no-image">on Gumroad</a>
to help support the &ldquo;Pydon'ts&rdquo; series of articles &#128170;.</p>
<!--^-->
</blockquote>
<h1>Beware, opinions ahead</h1>
<p>Idiomatic code, readable code, &ldquo;Pythonic&rdquo; code, elegant code,
these are all subjective things.
That means that whatever I write about these topics will never
be 100% consensual.
In other words, you might disagree.</p>
<p>I am fine with the fact that there are people who disagree with me,
and I do invite you to make yourself heard, maybe by writing me
or leaving a comment on the blog &ndash; diversity of points of view
is enriching.</p>
<p>I just want to let you know that this Pydon't might not be a good read
for you if you can't stand the fact that other people might think
differently from you &#128578;.</p>
<h1>Elegance is not a dispensable luxury</h1>
<p>Let me be honest with you:
when I was preparing my talk, and preparing this Pydon't,
I thought that part of my argument about why elegance is important was going
to draw from my experience as a mathematician &ndash; when doing mathematics,
people usually strive for writing elegant proofs, constructing simple arguments,
finding even simpler counter-examples to others' arguments, etc.</p>
<p>Then,
I found a quote by a respectable computer scientist that made this connection for me,
and I felt much more confident with the parallel I was trying to establish.
Edsger W. Dijkstra, a Dutch computer scientist,
after which the "[Dijkstra algorithm][dijkstra-alg]" was named, wrote:</p>
<blockquote>
<p>&ldquo;How do we convince people that in programming simplicity and clarity &ndash;
in short: what mathematicians call "elegance" &ndash;
are not a dispensable luxury, but a crucial matter that decides between success and failure?&rdquo;</p>
<p>&#8213; Edsger W. Dijkstra, "Selected Writings on Computing: A Personal Perspective", p347.</p>
</blockquote>
<p>I think Dijkstra's quote says it all:
simple and clear code is elegant code.
And this these are very desirable properties to have in code.
In fact, a little bit further down the page, Dijkstra adds</p>
<blockquote>
<p>&ldquo;[...] in the case of software unreliability is the greatest cost factor.
It may sound paradoxical, but a reliable (and therefore simple) program
is much cheaper to develop and use than a (complicated and therefore) unreliable one.&rdquo;</p>
</blockquote>
<p>From my experience, people mistake <em>beginner-level</em> code for <em>simple</em> and <em>clear</em> code,
and that is something very dangerous, in my opinion.</p>
<p>Don't get me wrong, there is nothing inherently wrong with beginner-level code,
we all write it when we are learning.
What is wrong is...</p>
                
            - [__name__ dunder attribute | Pydon't](https://mathspp.com/blog/pydonts/name-dunder-attribute) (Mon Jun 28 2021 10:00 PM)

 > 
                
                                <img alt="" src="https://mathspp.com/images/8/a/a/5/0/8aa5031d1bb564ecff477cd401b673a9eacc87c5-thumbnail.png" />
                                <p>This Pydon't walks you through the usages of the
<code>__name__</code> dunder method and how to use it effectively.</p>

<p><img alt="A Python code snippet that uses __name__." src="/user/pages/02.blog/04.pydonts/name-dunder-attribute/thumbnail.svg"></p>
<p>(If you are new here and have no idea what a Pydon't is, you may want to read the
<a href="/blog/pydonts/pydont-manifesto">Pydon't Manifesto</a>.)</p>
<h1>Introduction</h1>
<p>In this Pydon't we will take a look at the <code>__name__</code> attribute.
If you Google it, you will find a ton of results explaining <em>one</em>
use case of the <code>__name__</code> attribute, so in this Pydon't
I'll try to tell you about another couple of use cases
so that you learn to use <code>__name__</code> effectively in your Python programs.</p>
<p>In this Pydon't, you will:</p>
<ul><li>learn about the idiomatic usage of <code>__name__</code> to create &ldquo;main&rdquo; functions in Python;</li>
<li>learn about the read-only attribute <code>__name__</code> that many built-in objects get;</li>
<li>see how <code>__name__</code> is used in a convention involving logging; and </li>
<li>see some code examples of the things I will be teaching.</li>
</ul><!--v--><blockquote>
<p>You can now get your copy of the ebook &ldquo;Pydon'ts &ndash; Write beautiful Python code&rdquo; <a href="https://gum.co/pydonts" target="_blank" rel="nofollow noopener noreferrer" class="external-link no-image">on Gumroad</a>
to help support the series of &ldquo;Pydon't&rdquo; articles &#128170;.</p>
<!--^-->
</blockquote>
<h1>What is <code>__name__</code>?</h1>
<p><code>__name__</code> is a special attribute in Python.
It is special because it is a dunder attribute,
which is just the name that we give, in Python,
to attributes whose names start and end with a double underscore.
(I explain in greater detail what a dunder attribute/method
is in <a href="/blog/pydonts/usages-of-underscore#leading-and-trailing-double-underscores">a previous Pydon't</a>.)</p>
<p>You can <a href="https://docs.python.org/3/search.html?q=__name__&amp;check_keywords=yes&amp;area=default" target="_blank" rel="nofollow noopener noreferrer" class="external-link no-image">look <code>__name__</code> up in the Python documentation</a>,
and you will find two main results that we will cover here.
One of the results talks about <code>__main__</code> as a module attribute,
while the other result talks about <code>__main__</code> as an attribute
to built-in object types.</p>
<h1>The module attribute <code>__name__</code>
</h1>
<p>The most commonly known use case for <code>__name__</code> is as a module attribute,
when using <code>__name__</code> to create &ldquo;main&rdquo; functions in Python.
What this means is that you can use <code>__name__</code> to determine programmatically
if your code is being ran directly as a script or if it is being imported
from another module.</p>
<p>How can we do this?
Simple!</p>
<p>Go ahead and write the following line in your <code>print_name.py</code> file:</p>
<pre><code class="language-py">print(__name__)</code></pre>
<p>Now open your command line and run the script:</p>
<pre><code class="language-bash"> &gt; python print_name.py
__main__</code></pre>
<p>What this is showing you is that the attribute <code>__name__</code>
was automatically set to <code>"__main__"</code> when you ran your code
as a script.
This is relevant because that is <em>not</em> what happens when
you import your code from elsewhere.</p>
<p>As an example, go ahead and write the following line into your
<code>importer.py</code> file:</p>
<pre><code class="language-py">import print_name</code></pre>
<p>Then go ahead and run this new Python script:</p>
<pre><code class="language-bash"> &gt; python importer.py
print_name</code></pre>
<p>Where is that <code>"print_name"</code> being printed from?
Well, the <em>only</em> <code>print</code> statement you have is in the <code>print_name.py</code>
file, so that was definitely the place from where the printed value
came out.
Notice that some code got executed (and some things were
printed to the console) just by importing code from another module.</p>
<p>Also, notice that the value printed matches the name of the file...</p>
                
            - [Problem #039 – rope timer](https://mathspp.com/blog/problems/rope-timer) (Sat Jun 26 2021 10:00 PM)

 > 
                
                                <img alt="" src="https://mathspp.com/images/b/8/f/e/2/b8fe2c286152dc48f0a273cc27a41e4b412f159f-thumbnail.png" />
                                <p>You have two magical ropes that you can set on fire and you need
to count 45 minutes.
How do you do it?</p>

<figure class="image-caption"><img title="Photo of an hourglass by Aron Visuals on Unsplash." alt="" src="/images/8/c/e/a/d/8ceadcb9d516cbb3bfc004347490fdb6e77b610b-thumbnail.png"><figcaption class="">Photo of an hourglass by Aron Visuals on Unsplash.</figcaption></figure><h1>Problem statement</h1>
<p>You are given two magic ropes and a lighter.
The ropes are magic because you are told they burn in a weird way:
each rope takes exactly 1 hour to burn from end to end,
but they don't burn at a constant rate.
(What that means is that the time elapsed doesn't have to be
proportional to the length of burnt rope.
For example, it may happen that the first half of the rope
takes 35 min to burn,
then a huge portion of the remaining rope burns in 10 min,
and then the final tip of the rope takes 15 min to burn.)</p>
<p>Given two magic ropes like this, how do you use them to measure 45 minutes?</p>
<div class="notices blue">
<p>Give it some thought!</p>
</div>
<p>If you need any clarification whatsoever, feel free to ask in the comment section below.</p>
<h1>Solvers</h1>
<p>Congratulations to the ones that solved this problem correctly and, in particular, to the ones
who already sent me their correct solutions:</p>
<ul><li>Christ van W., The Netherlands;</li>
<li>Attila K., Hungary;</li>
<li>Ashok M., India;</li>
<li>David D., US;</li>
<li>Greg K., US;</li>
<li>Shivam T., US;</li>
<li>Marco M., Italy;</li>
<li>David H., Taiwan;</li>
<li>Cody B., US;</li>
</ul><p>(The list is in no particular order.)</p>
<p><a href="mailto:rodrigo@mathspp.com?subject=Solution%20to%20Problem%20#039%20%E2%80%93%20rope%20timer" class="mailto">Email me</a> your solution to get your name (or an alias) featured in here!</p>
<h1>Solution</h1>
<p>I find this problem to be really interesting!
The fact is that it looks like there is not much that we can do,
because the first thing that pops into our minds is to cut the rope
into portions, however, the problem statement tells us that the
time that a piece of rope takes to burn will not be proportional to its length.
Therefore, cutting the rope isn't an option.</p>
<p>Our only other option is to actually light the rope(s) on fire,
but that can't be <em>just</em> it, because a rope takes 60 minutes to burn
and we want to time 45 minutes.</p>
<p>The next step is realising that 45 minutes is <span class="mathjax mathjax--inline">\(3/4\)</span> of an hour,
and <span class="mathjax mathjax--inline">\(3/4 = 1/2 + 1/4\)</span>.
What is more, <span class="mathjax mathjax--inline">\(1/4 = (1/2)\times(1/2)\)</span>, i.e.,
three quarters of an hour is half an hour plus half of another half hour.
The recurring theme here is halves.
Therefore, it might be a good idea if we reframe the problem.
Instead of trying to measure a specific amount of time with the burning
of the ropes, can you do something to the rope so that it measures exactly
half of the total time that the rope could burn for?</p>
<p>In other words, if a rope takes a full <span class="mathjax mathjax--inline">\(x\)</span> minutes to burn,
how could you work with that rope in order to measure <span class="mathjax mathjax--inline">\(x/2\)</span> minutes?</p>
<p>Give it some thought.</p>
<p>If you light up the rope on both ends,
then it will burn for exactly half of the time!
So, if...</p>
                
            - [Usages of underscore | Pydon't](https://mathspp.com/blog/pydonts/usages-of-underscore) (Mon Jun 21 2021 10:00 PM)

 > 
                
                                <img alt="" src="https://mathspp.com/images/c/3/7/e/8/c37e832dd114024123030d4a37329c96a0312848-thumbnail.png" />
                                <p>The purpose of this Pydon't is to show you what underscores
are used for in Python, and to show you how to write
more idiomatic code with them.</p>

<p><img alt="A Python code snippet that shows the use of the underscore in the session." src="/user/pages/02.blog/04.pydonts/usages-of-underscore/thumbnail.svg"></p>
<p>(If you are new here and have no idea what a Pydon't is, you may want to read the
<a href="/blog/pydonts/pydont-manifesto">Pydon't Manifesto</a>.)</p>
<h1>Introduction</h1>
<p>In this Pydon't we will take a look at all the use cases there are
for <code>_</code> in Python.
There are a couple of places where <code>_</code> has a very special role
syntactically, and we will talk about those places.
We will also talk about the uses of <code>_</code> that are just conventions
people follow, and that allow one to write more idiomatic code.</p>
<p>In this Pydon't, you will:</p>
<ul><li>learn about the utility of <code>_</code> in the Python REPL;</li>
<li>learn what <code>_</code> does when used as a prefix and/or suffix of a variable name:
<ul><li>a single underscore used as a suffix;</li>
<li>a single underscore used as a prefix;</li>
<li>double underscore used as a prefix;</li>
<li>double underscore used as a prefix and suffix;</li>
</ul></li>
<li>see the idiomatic usage of <code>_</code> as a &ldquo;sink&rdquo; in assignments;</li>
<li>and understand how that was extended to <code>_</code>'s role in the new <code>match</code> statement;</li>
<li>see the idiomatic usage of <code>_</code> in localising strings; and</li>
<li>learn how to use <code>_</code> to make your numbers more readable.</li>
</ul><!--v--><blockquote>
<p>You can now get your copy of the ebook &ldquo;Pydon'ts &ndash; Write beautiful Python code&rdquo; <a href="https://gum.co/pydonts" target="_blank" rel="nofollow noopener noreferrer" class="external-link no-image">on Gumroad</a>
to help support the series of &ldquo;Pydon't&rdquo; articles &#128170;.</p>
<!--^-->
</blockquote>
<h1>Recovering last result in the session</h1>
<p>Have you ever called a slow function in the Python session and then lost the return
value because you forgot to assign it to a variable?
I know I have done that countless times!
Because of people like (you and) me, someone made the <em>best</em> decision ever,
and decided that <code>_</code> can be used in the Python session to refer to the
last return result:</p>
<pre><code class="language-py">&gt;&gt;&gt; 1 + 1
2
&gt;&gt;&gt; _
2
&gt;&gt;&gt; sum(range(100_000_000))     # Takes a couple of seconds to finish.
4999999950000000
&gt;&gt;&gt; _
4999999950000000
&gt;&gt;&gt; save_for_later = _
&gt;&gt;&gt; save_for_later
4999999950000000</code></pre>
<p>This prevents you from having to re-run the previous line of code,
which is especially helpful if the previous line of code takes some
time to finish, if it had side-effects that you don't want to trigger
again, or even if it can't be re-run (e.g. because you deleted a file
or because you exhausted an iterable).</p>
<p>So, next time you are playing around in the interpreter session and forget
to assign the result of a function call, or some other piece of code,
remember to use <code>_</code> to refer back to it.</p>
<p>Notice that if you explicitly assign to <code>_</code>,
then the value you assign will stay there until you explicitly delete it.
When you delete it, then <code>_</code> will go back to referring to the last
returned result:</p>
<pre><code class="language-py">&gt;&gt;&gt; _ = "hey"
&gt;&gt;&gt; "_ was explicitly assigned."
'_ was explicitly assigned.'
&gt;&gt;&gt; _
'hey'
&gt;&gt;&gt; del _
&gt;&gt;&gt; "_ is no...</code></pre>
                
            <!-- BLOG-POST-LIST:END -->

<br />
<br />

![](https://github-readme-stats.vercel.app/api?username=RojerGS&hide=stars&count_private=true&show_icons=true)
