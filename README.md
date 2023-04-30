Download Link: https://assignmentchef.com/product/solved-cs217-assignment-1-string-manipulation-functions-morse-code-and-magic-square
<br>
<h1>Q1: String manipulation functions</h1>

Write the implementation of the following functions:

<table width="627">

 <tbody>

  <tr>

   <td width="193">int         Strlen ( char ∗s1 )/∗Returns the length                   of{}</td>

   <td width="79">the        string</td>

   <td width="81">in number</td>

   <td width="24">of</td>

   <td width="251">characters . ∗/</td>

  </tr>

  <tr>

   <td width="193"> </td>

   <td width="79"> </td>

   <td width="81"> </td>

   <td width="24"> </td>

   <td width="251"> </td>

  </tr>

  <tr>

   <td width="193">char ∗Strcpy ( char ∗s1 ,</td>

   <td width="79">const char</td>

   <td width="81">∗s2 )</td>

   <td width="24"> </td>

   <td width="251"> </td>

  </tr>

  <tr>

   <td width="193">/∗Copies         string     s2        into{}</td>

   <td width="79">array s1 .</td>

   <td width="81">The value</td>

   <td width="24">of</td>

   <td width="251">s1    is      returned . ∗/</td>

  </tr>

 </tbody>

</table>

1

2

3

4

1

2

3

4

1 char ∗Strncpy ( char ∗s1 , const char ∗s2 , size t n ) 2 /∗Copies at most n characters of string s2 into array s1 .

<h2>3       The value      of    s1    is      returned . ∗/</h2>

{

1             char ∗StrCat ( char ∗s1 , const char ∗s2 ) 2              /∗Appends string    s2 to array s1 .

3 The f i r s t character of s2 overwrites 4 the terminating null character of s1 .

<h2>5       The value      of    s1    is      returned . ∗/</h2>

{ 1 char ∗StrnCat( char ∗s1 , const char ∗s2 , size t n ) 2 /∗Appends at most n characters of string s2 to array s1 .

<h2>3             The f i r s t           character             of            s2           overwrites          the terminating 4 null        character             of            s1 . The 5             value     of            s1           is            returned . ∗/</h2>

{

1 int StrCmp( const char ∗s1 , const char ∗s2 ) 2 /∗Compares the string s1 with the string s2 .

<h2>3             The function       returns  0 ,           less than 0 or              greater 4              than 0    i f s1           is            equal to ,              less than or  greater 5              than s2  , respectively . ∗/</h2>

{

1              int StrnCmp( const char ∗s1 ,                 const char ∗s2 ,             size t n )

<h2>2             /∗Compares up to n characters     of            the         string 3 s1 with the          string    s2 . The function       returns  0 , 4        less        than 0 or              greater than 0     i f            s1           is equal 5  to ,          less        than or  greater than s2 , respectively . ∗/</h2>

{

<table width="627">

 <tbody>

  <tr>

   <td colspan="2" width="627">char ∗∗StrTok( char ∗s1 , const char s2 ) /∗A call to StrTok breaks string s1 into</td>

  </tr>

  <tr>

   <td width="256">‘ ‘ tokens ‘ ‘           ( logical        pieces         such</td>

   <td width="371">as words</td>

  </tr>

  <tr>

   <td width="256">in a line of            text ) separated by contained           in char s2∗/{</td>

   <td width="371">character</td>

  </tr>

  <tr>

   <td width="256">int         StrFind ( char ∗s1 ,               char ∗s2 )/∗Searches the             string     s1    for      the</td>

   <td width="371">f i r s t        occurrence</td>

  </tr>

  <tr>

   <td width="256">of     the      string         s2 and returns          itsi f             s2 not found returns −1.∗/{</td>

   <td width="371">starting            index ,</td>

  </tr>

 </tbody>

</table>

1

2

3

4

5

1

2

3

4

1            char ∗ SubStr ( char ∗ ,             int pos ,       int     len )

<h2>2         /∗This function                returns a newly constructed</h2>

3 string variable with its value initialized 4 to a copy of a substring of this variable . 5 The substring is the portion of the string

<h2>6             that        starts     at            character             position ‘ ‘ pos ‘ ‘ and 7      spans     ‘ ‘ len ‘ ‘ characters           ( or         until      the end 8              of            the         string ,   whichever comes f i r s t ). ∗/</h2>

{

<h1 style="margin-bottom: 0.540791em;font-size: 2.61792em"></h1>

Figure 1: A mapping table between English Alphabets and Morse codes. Source: http://en.wikipedia.org/ wiki/Morse code

<h1>Q2:</h1>

<h1>Morse Code</h1>

Morse code has been one of the most basic communication protocol and still used to convey SOS messages and other urgent communication. In Morse code each English alphabet is encoded by a sequence of ’.’ and ’-’, see Figure 1 for complete mapping between English alphabets and Morse codes. Letters are separated by spaces and words by ”/”. Your task is to design a program that can (i)convert any given string into a Morse code sequence <em>char* convertToMorseCode(char*) </em>and (ii) a Morse code sequence to a string. <em>char* convertToString(char*) </em><strong>You are not authorized to use </strong><em>string </em><strong>data type, however you can use </strong><em>char*</em>

<h1>Q3: Magic Squares</h1>

In this question your goal is to write code for solving magic square (for details read the attached file magicsquare.pdf) using 2-D pointers. Your function should take the the dimension of magic square as input and then solve the magic square for given dimension. You are required to return a 2d pointer to an integer.

1           int ∗∗ magicSquare ( int          size )

<h2>2             /∗This function  returns a 2d pointer         that dynamically 3            allocates a matrix of size        passed as arguments 4     and store magic square    in           allocated              matrix . ∗/</h2>

{

<h1>Q4: Text Analysis</h1>

The availability of computers with string-manipulation capabilities has resulted in some rather interesting approaches to analyzing the writings of great authors. This exercise examines three methods for analyzing texts with a computer. <strong>You have to use char * for following exercises.</strong>

<ol>

 <li>Write a function that receives a string consisting of several lines of text and returns an array indicating the number of occurrences of each letter of the alphabet in the text. For example, the phrase To be, or not to be: that is the question: contains one a, two bs, no cs, and so on.</li>

</ol>

1 void countLetters ( char ∗string , int ∗&amp;array , int &amp; size ) 2 /∗Parameters :

<ul>

 <li>Input :</li>

 <li>char ∗ : a multiline string 5 Output :</li>

</ul>

<h2>6  int          ∗: an array           containing           counts   of each  letter , 7 to be allocated    in     function 8            int          :              array     size        ∗/</h2>

{

<ol start="2">

 <li>Write a function that receives a string consisting of several lines of text and returns an array indicating the number of one-letter words, two-letter words, three-letter words, and so on, appearing in the text. For example, the phrase Whether this nobler in the mind to suffer contains 2, 3, 4, etc. length words.</li>

</ol>

1 void countWordsBasedOnLength( char ∗string , int ∗&amp;array/∗to be allocated ∗/ , 2 int &amp; size /∗updated array size ∗/) 3 /∗Parameters :

<ul>

 <li>Input :</li>

 <li>char ∗ : a multi−line string 6 Output :</li>

</ul>

<h2>7  int          ∗: an array           containing           counts   of each  different              length words , 8   to be allocated    in           function 9            int          :              array     size        ∗/</h2>

{

<ol start="3">

 <li>Write a function that receives a string consisting of several lines of text and returns arrays indicating unique words and the number of occurrences of each unique word in the text along with their size.</li>

</ol>

<ul>

 <li>void countingUniqueWords( char ∗string , char ∗∗&amp;uwords/∗ l i s t  of unique words ; ∗/ ,</li>

 <li>int ∗&amp;array/∗to be allocated ∗/ , int &amp; size /∗updated array size ∗/) 3 /∗Parameters :</li>

 <li>Input :</li>

 <li>char ∗ : a multiline string 6 Output :</li>

</ul>

<h2>7  char ∗∗: an array of unique words 8             int          ∗:            their      counts 9               int     : number of unique words∗/</h2>

{