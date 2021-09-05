# Label search
## One label

<pre>blogURL/search/label/<b>Label</b></pre>

<pre>blogURL/search?q=label:<b>Label</b></pre>

<pre>blogURL/search?q=label:"<b>Label with multiple words</b>"</pre>

## Multiple label

<pre>blogURL/search/label/<b>Label1</b>+<b>Label2</b>+<b>Label3</b></pre>

# Search a Term within Specific Label
<pre>
blogURL/search?q=<b>term</b>+label:"Lyric and Chord"
</pre>
Note that a space in a URL will be converted to `+` sign. When implemented in a from, you need to stop form default behaviour using `event.preventDefault`, concat submitted search term with label query by a space character, then programatically submit the form. Additionally, you can reset the search input value back to before it was concated with extra label parameter after submmitting the form. 

For example, the URL before the form is submmited should be :
```
blogURL/search?q=<b>term</b> label:"Lyric and Chord"
```
