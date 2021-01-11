# Tutorial

md stands for mark down, and is an easy way to format the text; has shortcuts <p>
one hashtag for a main header --> #Demo made a main header <p>
<p>
README.md is the file that github shows when you enter a repository. <p>
<p>
when commiting (saving) a file, there is a description box with default text in it saying "create README.md" or "Update README.md" to describe the change. If you want another description, type it in. (plus there's an optional extended description) <p> 
use html for commands such as &lt;p&gt; <p>

##Entities
certain signs, such as &lt; &gt; are considered command prompts around certain characters. To make them show up in text, need to use their HTML entities; either &entity_name or &#entity_number. for &lt; the entity name is lt; and its entity number is 60. for &gt; the entity name is gt; and its number is 62. for &amp; the name is amp;
<p>more on entities; https://www.w3schools.com/html/html_entities.asp
<p> in commits; anything with + and in green is stuff that was added after the previous commit, - and red is stuff that was deleted, white is everything that remained unchanged
<p>
note: chose 'cache data for faster operations' when installing github, therefore might be a reason if it works slowly
<p>
open terminal command  "git clone" followed by clone link from github to clone something to git <p>

creating ssh keys; need to have ssh-keygen.exe; mac + linux git files download it for you, windows should already have it, if program says can't find ssh-keygen, need to download it or find it in programs, then go to ... and add path to where the ssh folder is located, so that in the future, git would search in that file too. <p>
type: ssh-keygen -t rsa -b 4069 -C "email@example.com", wait until it asks to "enter file in which to save key" eg. testkey saved in /.ssh/id_rsa
<p>
<p>just highlighting smth in terminal adds it to clipboard - don't need ctrl +c bc that means smth else
