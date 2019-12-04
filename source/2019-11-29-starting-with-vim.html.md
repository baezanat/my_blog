---

title: Starting with VIM
date: 2019-11-29 10:05 CET
tags: vim

---

Are you thinking about trying VIM? I am a newbie to coding in general, and I've only been using VIM for about 3 weeks, but I already love it. If you're looking for some editing wizardry and want some tips to get started, please read on.

<div class="container">
  <img src="/media/starting_with_vim/magic.jpg" alt="sign with the words 'in pursuit of magic'" class="banner">
</div>

&nbsp;
&nbsp;

## 1. Why VIM  

There are good reasons both to try VIM and to stick to other editors. Here are the reasons that brought me to VIM:  

1. Popular editors come in and out of existence fairly often, unable to survive big technology shifts. These changes are disruptive; you have to learn to use a new text editor and build muscle memory with it. VIM/ VI has been around for about 40 years and has withstood all kinds of major changes, so could actually be a text editor for life.
2. It takes time to learn VIM, but it is clear from seeing VIM wizards use VIM that you can get to a very high level of proficiency with it. I like the prospect of reaching mastery with my tools.  
3. You can configure VIM to your needs with a very high level of precision.
4. I'm just a sucker for new, hard things to learn.  

&nbsp;
&nbsp;

## 2. Tips to Get Started  

The first thing you need is to learn the basic commands to get around VIM. The <a class="link" href="https://www.openvim.com/">VIM TUTOR</a> is a good place to start.

After that, you need to practice on your own.   
- Make a simple practice text file and play around with it. Practic makes perfect.  

- I recommend keeping a file with the most useful commands you've found. As you find new things you need and figure out how to do them with VIM, you'll expand your list into a very useful cheat sheet.

I got some great ideas to configure VIM for my needs from <a href="https://www.udemy.com/course/vim-training-course-ruby-developers/learn/lecture/6174330?start=135#overview" class="link">this udemy course</a> for Ruby developers, since my current work is mostly with Ruby. If you'd like to follow a structured course, <a class="link" href="https://www.udemy.com/course/vim-commands-cheat-sheet/">this</a> looks like a good general introduction, and it's only $10. In general though, you'll learn the most from simply using vim as much as you can and solving problems as they arise. You can find great resources at <a href:"www.vim.org" class="link">vim online</a>. Usually, though, I just google search what I need and always find a solution.  
 
 &nbsp;
 &nbsp;

## 3. Some Commands to Get Started  

### Help  

:h          Get help  

:bd         Exit help  


### Navigation

<table>
<tbody>
<tr class="odd">
<td>w, b, e</td>
<td>Navigate between words</td>
</tr>
<tr class="even">
<td>0, $</td>
<td>Beginning / End of current line</td>
</tr>
<tr class="odd">
<td>&lt;6 - G&gt; or &lt;:6&gt;</td>
<td>Jump to line 6</td>
</tr>
<tr class="even">
<td>B, W</td>
<td>Previous/ Next section</td>
</tr>
<tr class="odd">
<td>H, M, I</td>
<td>Top /middle/ bottom of screen</td>
</tr>
<tr class="even">
<td>5w</td>
<td>Forward 5 words</td>
</tr>
<tr class="odd">
<td>5l, 5h</td>
<td>Forward / Back 5 letters</td>
</tr>
<tr class="even">
<td>5j, 5k</td>
<td>Forward 5 lines / Up 5 lines</td>
</tr>
<tr class="odd">
<td>F + &lt;letter&gt;</td>
<td>Forward to next &lt;letter&gt; (case sensitive)</td>
</tr>
<tr class="even">
<td>gg/ G</td>
<td>Top/ end of file</td>
</tr>
<tr class="odd">
<td>%</td>
<td>Jump to matching parenthesis/ bracket</td>
</tr>
</tbody>
</table>
<p></p>


<h3>Editing</h3>

<p></p>
<table>
<tbody>
<tr class="odd">
<td>u, &lt;ctr + R&gt;</td>
<td>Undo / Redo</td>
</tr>
<tr class="even">
<td>i, a</td>
<td>Insert text at cursor /position insert text after letter under cursor</td>
</tr>
<tr class="odd">
<td>&lt;shift + i&gt;, &lt;shift+ a&gt;</td>
<td>Insert text at beginning / End of line</td>
</tr>
<tr class="even">
<td>o, O</td>
<td>Insert text in next / Previous line</td>
</tr>
<tr class="odd">
<td>3i&lt;text&gt;</td>
<td>Inserts &lt;text&gt;&lt;text&gt;&lt;text&gt;</td>
</tr>
<tr class="even">
<td>v&gt;, v&lt;</td>
<td>Change indentation (add to right/ move back to left)</td>
</tr>
<tr class="odd">
<td>ci”</td>
<td>Change everything within quotes</td>
</tr>
<tr class="even">
<td>Cit</td>
<td>Change everything within tags (e.g. HTML)</td>
</tr>
<tr class="odd">
<td>cw, c5w, C</td>
<td>Change word / change 5 words / to end of line</td>
</tr>
<tr class="even">
<td>X, x</td>
<td>Delete to left of cursor / Delete under cursor</td>
</tr>
<tr class="odd">
<td>s</td>
<td>Delete character under cursor and enter Insert mode</td>
</tr>
<tr class="even">
<td>r</td>
<td>Replace character under cursor</td>
</tr>
<tr class="odd">
<td>d</td>
<td>Delete current and left character</td>
</tr>
<tr class="even">
<td>db, dw</td>
<td>Delete to beginning / end of current word</td>
</tr>
<tr class="odd">
<td>cw</td>
<td>Delete entire word</td>
</tr>
<tr class="even">
<td>d^</td>
<td>Delete back to first non-white-space character</td>
</tr>
<tr class="odd">
<td>d0, d$</td>
<td>Delete to beginning / to end of line</td>
</tr>
<tr class="even">
<td>dd</td>
<td>Delete current line</td>
</tr>
<tr class="odd">
<td>J</td>
<td>Join line below</td>
</tr>
<tr class="even">
<td>d5</td>
<td>Delete 5 lines</td>
</tr>
<tr class="odd">
<td>d5G</td>
<td>Deletes up to (and including) line number 5</td>
</tr>
<tr class="even">
<td>dgg, dG</td>
<td>Delete to beginning / end of file</td>
</tr>
<tr class="odd">
<td>:g/&lt;pattern&gt;/d</td>
<td>Delete all items that start with &lt;pattern&gt;</td>
</tr>
</tbody>
</table>
<p></p>

<h3>Select</h3>


<p></p>
<table>
<tbody>
<tr class="odd">
<td>V, v</td>
<td>Select a line / a range of text</td>
</tr>
<tr class="even">
<td>&lt;ctrl + v&gt;</td>
<td>Select a column / block</td>
</tr>
<tr class="odd">
<td>gv</td>
<td>Reselect a block</td>
</tr>
<tr class="even">
<td>vw, v5w</td>
<td>Select a word / Select 5 words</td>
</tr>
<tr class="odd">
<td>vt,</td>
<td>Select till ,</td>
</tr>
<tr class="even">
<td>v/&lt;text&gt;</td>
<td>Select elements in paragraph</td>
</tr>
<tr class="odd">
<td>ggVG</td>
<td>Select all</td>
</tr>
</tbody>
</table>
<p></p>

<h3>Search</h3>


<p></p>
<table>
<tbody>
<tr class="odd">
<td>f&lt;text&gt;, 3f&lt;text&gt;</td>
<td>Finds next / 3<sup>rd</sup> occurrence of &lt;text&gt; </td>
</tr>
<tr class="even">
<td>\*, #</td>
<td>Find next / previous occurrence of word under cursor</td>
</tr>
<tr class="odd">
<td>/&lt;word&gt;</td>
<td>Search for &lt;word&gt; in file</td>
</tr>
<tr class="even">
<td>?&lt;word&gt;</td>
<td>Search backward</td>
</tr>
<tr class="odd">
<td>n, N</td>
<td>Find previous / next result</td>
</tr>
<tr class="even">
<td>ggn, GN</td>
<td>Go to First / Last result</td>
</tr>
<tr class="odd">
<td>:noh</td>
<td>Remove highlighting</td>
</tr>
<tr class="even">
<td><p></p>
<p>:%s/&lt;text1&gt;/&lt;text2&gt;/gc</p></td>
<td><p>Search and Replace</p>
<p>Search for &lt;text1&gt; and <em>globally</em> replace with &lt;text2&gt;,<br />
ask for confirmation</p></td>
</tr>
</tbody>
</table>
<p></p>

<h3>Copy and Paste</h3>


<p></p>
<table>
<tbody>
<tr class="odd">
<td>yy or Y</td>
<td>Copy entire line</td>
</tr>
<tr class="even">
<td>p</td>
<td>paste</td>
</tr>
<tr class="odd">
<td>&quot;*y</td>
<td>Copy to * (clipboard)</td>
</tr>
<tr class="even">
<td>&quot;*p</td>
<td>Paste from clipboard</td>
</tr>
</tbody>
</table>
<p></p>

<p>----------------------------------------------------------------------------------------------</p>
