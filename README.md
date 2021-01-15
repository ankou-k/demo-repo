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

creating ssh keys; need to have ssh-keygen.exe; mac + linux git files download it for you, windows should already have it, if program says can't find ssh-keygen, need to download it or find it in programs, then go to computer advanced properties and add path to where the ssh folder is located, so that in the future, git would search in that file too. <p>
type: ssh-keygen -t rsa -b 4069 -C "email@example.com", wait until it asks to "enter file in which to save key" enter the file into which to save the key under, with last line after \ being the name under which the key will be saved 
"/.ssh/id_rsa" is just the placeholder for the future names of the files
<p> SHA256:/uWzOtgFYUeRaW29f7vHUvQgvEMTR94Nk8RloPFuoZo mayya@LenovoE14
.pub key can be shared, the other key is private and should not be shared to any other place/machine
put public key on github, then to push something from the machine to github use the private key to demonstrate that it's you, since only this private key could've generated that public key

<p>just highlighting smth in terminal adds it to clipboard - don't need ctrl +c bc that means smth else

path=%path%C:\"Example with space"\file
creates a new path for the current session (to make permanent have to go to computer properties)
the % around path means to add the stuff after it to the existing path value, like in java you'd write path += C:\file
directories with spaces need to have "" around them since space means next argument (irony; Windows creates directories titled "Program Files")

windows uses back slashes \ to indicate different level of directory, while unix uses /
therefore, when using the command ffind (which is my copy of the unix find tool, which finds files rather than text in files like the windows find tool) the results look like ./file/smallFile
but when i want to do something like add a path or move to a different directory, i'm communicating with the windows tools so i use \

in unix, back slash \ changes the meaning of the symbol following it; while in printf it adds meaning to the subsequent symbol, in unix it acts as special symbol escape aka the subsequent symbol is just another line of text rather than a command. vscode uses linux syntax in its settings (eg git.path) since vscode is a transplatform program and needs to operate on both. so in git.path when indicating the path of git, the location which on windows must be found under C:\Files would be written as C:\\Files to null the "symbol escape" function of the second slash

the terminal is a seperate program from vscode, so the settings from vscode don't transfer to the terminal and specifying the git path for vscode did not make the terminal respond to "git" until the git path was added in the computer settings
terminal can be powershell or cmd (older) which have different syntax, for example there is no path command in powershell. add terminal with the + button, choose default shell in drop down menu

use * to indicate any other text eg. '\*hello\*' (without the backslashes) would mean that whatever command would include everything that has 'hello' in it; "hello", "1hello" "7hello7"
so to find files that have ".txt" in it, would use ffind . -name "\*.txt" (the . is in place of directory name, can indicate another directory) need "" around the name if have * in there because otherwise, if there's a file in the main directory that contains ".txt" the shell would insert the text before .txt in place of * before passing it into the ffind. ex if have "wow.txt" and type ffind . -name *.txt it is the same as typing ffind . -name wow.txt b/c the wow was put in place of * before the ffind function was run
