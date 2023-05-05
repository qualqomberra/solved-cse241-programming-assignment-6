Download Link: https://assignmentchef.com/product/solved-cse241-programming-assignment-6
<br>
<h1>Description</h1>

<ul>

 <li>This is an individual assignment. Please do not collaborate</li>

 <li>If you think that this document does not clearly describes the assignment, ask questions before its too late.</li>

</ul>

This assignment is about using C++ STL, exception handling and/or creating Class templates.

<ul>

 <li>Your program reads two files:

  <ul>

   <li>txt</li>

   <li>txt</li>

  </ul></li>

 <li>According to content in data.txt, the program utilizes necessary STL classes and/or user-created classes for a catalog representation.</li>

 <li>Your program creates a log file(output.txt) for certain steps of operations performed on catalog. <strong>txt</strong></li>

 <li>This file holds information about a catalog. A catalog can be one of the following:

  <ul>

   <li>Book catalog</li>

   <li>Music catalog</li>

   <li>Movie catalog</li>

  </ul></li>

 <li>The type of the catalog is specified in the first line of data.txt</li>

</ul>

<h2>Book Catalog</h2>

<ul>

 <li>Each line in a book catalog keeps information about a book.</li>

 <li>Format:</li>

</ul>

&lt;title&gt; &lt;authors&gt; &lt;year&gt; &lt;tags&gt;

<ul>

 <li>Example: Contents of data.txt for a book catalog</li>

 <li>book</li>

 <li>“Hilbert Spaces With Applications” “Lokenath Debnathl, Piotr Mikusinski” “2005” “Mathematics,</li>

</ul>

<em>,</em><em><sub>→ </sub></em>Set Theory”

<ul>

 <li>“The Neolithic Revolution in the Near East: Transforming the Human Landscape” “Alan H. Simmons”</li>

</ul>

<em>,</em><em><sub>→ </sub></em>“2011” “Social Science, Anthropology, Cultural, General, Archaeology”

<ul>

 <li>“Learning Flask Framework” “Matt Copperwaite, Charles Leifer” “2015” “Computers, Programming</li>

</ul>

<em>,</em><em><sub>→ </sub></em>Languages, Python, Internet, Application Development, Web, Web Programming”

<ul>

 <li>“Graphics Gems V” “Alan W. Paeth” “1995” “”</li>

</ul>

<h2>Music Catalog</h2>

<ul>

 <li>Each line in a music catalog keeps information about a music album.</li>

 <li>Format:</li>

</ul>

&lt;title&gt; &lt;artists&gt; &lt;year&gt; &lt;genre&gt;

<ul>

 <li>Example: Contents of data.txt for a music catalog</li>

 <li>music</li>

 <li>“Professor Satchafunkilus and the Musterion of Rock” “Joe Satriani” “2008” “Guitar Virtuoso”</li>

 <li>“Physical Graffiti” “Led Zeppelin” “1975” “Rock”</li>

 <li>“Witchdoctor’s Son” “Okay Temiz, Johnny Dyani” “2017” “Jazz, Fusion”</li>

 <li>“Return Of The Mother Head’s Family Reunion” “Richie Kotzen” “2007” “Rock, Guitar Virtuoso”</li>

</ul>

<h2>Movie Catalog</h2>

<ul>

 <li>Each line in a movie catalog keeps information about a movie.</li>

 <li>Format:</li>

</ul>

&lt;title&gt; &lt;director&gt; &lt;year&gt; &lt;genre&gt; &lt;starring&gt;

<ul>

 <li>Example: Contents of data.txt for a movie catalog</li>

 <li>movie</li>

 <li>“The Lord of the Rings: The Fellowship of the Ring” “Peter Jackson” “2001” “Adventure, Drama,</li>

</ul>

<em>,</em><em><sub>→ </sub></em>Fantasy” “Elijah Wood, Ian McKellen, Orlando Bloom”

<ul>

 <li>“Twelve Monkeys” “Terry Gilliam” “1995” “Mystery, Sci-Fi, Thriller” ” Bruce Willis, Madeleine</li>

</ul>

<em>,</em><em><sub>→ </sub></em>Stowe, Brad Pitt”

<ul>

 <li>“Perfume: The Story of a Murderer” ” Tom Tykwer” “2006” “Crime, Drama, Fantasy” “Ben Whishaw,</li>

</ul>

<em>,</em><em><sub>→ </sub></em>Dustin Hoffman, Alan Rickman”

<ul>

 <li>“Cold Mountain” “Anthony Minghella” “2003” “Adventure, Drama, History” ” Jude Law, Nicole</li>

</ul>

<em>,</em><em><sub>→ </sub></em>Kidman, Renee Zellweger” <strong>commands.txt</strong>

This file includes several commands which work on the catalog information you read from data.txt. Each line is a command. The following should be recognized:

<ul>

 <li>There are two commands.</li>

</ul>

search &lt;string&gt; in &lt;field&gt; sort &lt;field&gt; <strong>search command</strong>

<ul>

 <li>Format: search &lt;string&gt; in &lt;field&gt;</li>

 <li>Output:</li>

</ul>

This command returns a list of matched(partially or fully) entries (one entry in a line). Search should be limited to the field specified. Not found returns no line.

<ul>

 <li>Example:</li>

</ul>

search “Joe” in “artists” This returns the following line:

“Professor Satchafunkilus and the Musterion of Rock” “Joe Satriani” “2008” “Guitar Virtuoso” <strong>sort command</strong>

<ul>

 <li>Format: sort &lt;field&gt;</li>

 <li>Output:</li>

</ul>

This command returns a list of sorted entries (ascending order)

<ul>

 <li>Example:</li>

</ul>

sort “title”

This returns the following lines: 1 “Cold Mountain” “Anthony Minghella” “2003” “Adventure, Drama, History” ” Jude Law, Nicole

<em>,</em><em><sub>→ </sub></em>Kidman, Renee Zellweger”

<ul>

 <li>“Perfume: The Story of a Murderer” ” Tom Tykwer” “2006” “Crime, Drama, Fantasy” “Ben Whishaw,</li>

</ul>

<em>,</em><em><sub>→ </sub></em>Dustin Hoffman, Alan Rickman”

<ul>

 <li>“The Lord of the Rings: The Fellowship of the Ring” “Peter Jackson” “2001” “Adventure, Drama,</li>

</ul>

<em>,</em><em><sub>→ </sub></em>Fantasy” “Elijah Wood, Ian McKellen, Orlando Bloom”

<ul>

 <li>“Twelve Monkeys” “Terry Gilliam” “1995” “Mystery, Sci-Fi, Thriller” ” Bruce Willis, Madeleine</li>

</ul>

<em>,</em><em><sub>→ </sub></em>Stowe, Brad Pitt” <strong>output.txt</strong>

This file keeps the log of the operations. The following events should be recorded in the specified format:

<ul>

 <li>catalog read</li>

 <li>output of commands <strong>catalog read</strong></li>

 <li>First specify the type of the catalog.</li>

 <li>At the end, state the number of unique entries.</li>

</ul>

Catalog Read: music 4 unique entries <strong>output of commands</strong>

<ul>

 <li>State the command.</li>

 <li>Append its output.</li>

</ul>

search “Joe” in “artists”

“Professor Satchafunkilus and the Musterion of Rock” “Joe Satriani” “2008” “Guitar Virtuoso”

<h1>Exceptions</h1>

<ul>

 <li>Your program should catch certain exceptions and create log entries for them.</li>

 <li>You need to catch the following exceptions:</li>

</ul>

<h2>Missing field exception</h2>

<ul>

 <li>If any of the field in any entries is missing your program should omit that line and create an exception record in the log file.</li>

</ul>

Exception: missing field

<h2>Duplicate entry exception</h2>

<ul>

 <li>If the first field of any entries fully match, your program should create an exception for each repetition and log these instances in the log file.</li>

</ul>

Exception: duplicate entry

<h2>Wrong command exception</h2>

<ul>

 <li>If the command is not in the expected format(unrecognized field name, extra information etc…), log this instance as an exception. Exception: command is wrong</li>

</ul>

<strong>A full example.</strong>

<ul>

 <li>Suppose we are given the following data.txt file and commands.txt file:</li>

 <li>txt</li>

 <li>movie</li>

 <li>“The Lord of the Rings: The Fellowship of the Ring” “Peter Jackson” “2001” “Adventure, Drama,</li>

</ul>

<em>,</em><em><sub>→ </sub></em>Fantasy” “Elijah Wood, Ian McKellen, Orlando Bloom”

<ul>

 <li>“Twelve Monkeys” “Terry Gilliam” “1995” “Mystery, Sci-Fi, Thriller” ” Bruce Willis, Madeleine</li>

</ul>

<em>,</em><em><sub>→ </sub></em>Stowe, Brad Pitt”

<ul>

 <li>“Twelve Monkeys” “” “” “Sci-Fi, Thriller” ” Bruce Willis, Madeleine Stowe, Brad Pitt” 5 “Perfume: The Story of a Murderer” ” Tom Tykwer” “2006” “Crime, Drama, Fantasy” “Ben Whishaw,</li>

</ul>

<em>,</em><em><sub>→ </sub></em>Dustin Hoffman, Alan Rickman”

<ul>

 <li>“Twelve Monkeys” “” “” “Mystery, Sci-Fi, Thriller” ” Bruce Willis, Madeleine Stowe, Brad Pitt”</li>

 <li>“Cold Mountain” “Anthony Minghella” “2003” “Adventure, Drama, History”</li>

 <li>commands.txt</li>

 <li>search “Monkeys” in “title”</li>

 <li>search “Spice” in “type”</li>

 <li>sort “year”

  <ul>

   <li>The first line is movie. This means your application will going to run in movie organiser mode.</li>

   <li>Following is the log file for this example:</li>

   <li>txt 1 Catalog Read: movie</li>

  </ul></li>

 <li>Exception: duplicate entry</li>

 <li>“Twelve Monkeys” “” “” “Sci-Fi, Thriller” ” Bruce Willis, Madeleine Stowe, Brad Pitt”</li>

 <li>Exception: duplicate entry</li>

 <li>“Twelve Monkeys” “” “” “Mystery, Sci-Fi, Thriller” ” Bruce Willis, Madeleine Stowe, Brad Pitt”</li>

 <li>Exception: missing field</li>

 <li>“Cold Mountain” “Anthony Minghella” “2003” “Adventure, Drama, History”</li>

 <li>3 unique entries</li>

 <li>search “Monkeys” in “title”</li>

 <li>“Twelve Monkeys” “Terry Gilliam” “1995” “Mystery, Sci-Fi, Thriller” ” Bruce Willis, Madeleine</li>

</ul>

<em>,</em><em><sub>→ </sub></em>Stowe, Brad Pitt”

<ul>

 <li>Exception: command is wrong</li>

 <li>search “Spice” in “type”</li>

 <li>sort “year”</li>

 <li>“Twelve Monkeys” “Terry Gilliam” “1995” “Mystery, Sci-Fi, Thriller” ” Bruce Willis, Madeleine</li>

</ul>

<em>,</em><em><sub>→ </sub></em>Stowe, Brad Pitt”

<ul>

 <li>“The Lord of the Rings: The Fellowship of the Ring” “Peter Jackson” “2001” “Adventure, Drama,</li>

</ul>

<em>,</em><em><sub>→ </sub></em>Fantasy” “Elijah Wood, Ian McKellen, Orlando Bloom”

<ul>

 <li>“Perfume: The Story of a Murderer” ” Tom Tykwer” “2006” “Crime, Drama, Fantasy” “Ben Whishaw, <em>,</em><em><sub>→ </sub></em>Dustin Hoffman, Alan Rickman”</li>

</ul>