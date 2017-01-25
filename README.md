# markdown-practice
My lifelong quest to become the greatest master of markdown that the world has ever seen


https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet
A good markdown reference
http://www.markdowntutorial.com/conclusion/
A good basic markdown tutorial

##FORMATS:

~~Double-tilde will create a strikethrough~~

_italic text is surrounded by underscores_

**Bold text is surrounded by two asterisks**

_You can_ combine underscores and double-asterisks to make text both **bold and italic** in the same line

**_Combine them for text that is bold and italic_**

By the way, word wrap is ok to use for markdown, since it is not code

Use a Hash to make a header, you can make larger headers by adding another Hash... all the way up to seven hashes

####### Header 7
#### Header 4

You can italicize words in a header, although you can't make it bold

##### This _is_ a header!

To make an inline line, wrap texts in brackets, then parentheses  
[This link goes to google](www.google.com)

[**You can** make the text bold within a link description](www.google.com)

####Make a [link](www.google.com) within a header!

##REFERENCE LINKS:

Place a double bracketted linkname/link combo, but the link portion is a reference variable.
At the bottom of the document, the references variables are defined as links by linkname in brackets, followed by a colon, followed by the link

The reference link below is invisible when rendered

[this link is a reference][google]
[google]:www.google.com

##IMAGES:

Image begins with a !, then includes 'description' in brackets, then a pair of parentheses with the image url

![image of google logo description](https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png)

##IMAGE REFERENCE LINKS:

Same as reference links. A ! and bracket for description and reference variable, then another set with reference variable, colon, link

![image description][reference link]
[reference link]:https://www.google.com/images/branding/googlelogo/2x/googlelogo_color_272x92dp.png


##BLOCK QUOTES:

Preface a line with a greater-than caret >. Blank lines must be block quoted if they will be included in the block.

> The caret will carry over when word wrap is applied by a code editor.

multi-line block
> This is a block quoted line
>
> The block quote continues to here

Can include other formats in the block quote
> going to _italicize_ here


##LISTS:

Bullet lists: Preface line with a single asterisk and space

* First bullet list item
* Next bullet list item

Ordered lists: Number and period, then a space

1. First item
2. Second item
3. Third item

Can add formats within lists

1. Going to _italicize_ here

Grouping/Nesting lists:

Indent each asterisk for nested items by one space

* Main level
 * sub level 1
 * sub level 1
* back to main level
 * sub level 1
  * sub level 2

Paragraphs in list items:

Paragraph must start on a line all by itself underneath the bullet point but indented by AT LEAST ONE space

* List with paragraph beneath

 Two spaces could be used to to include this, but it will render the same.


##PARAGRAPHS:

Typing a singe line after another line will add an extra 'break' line when rendered. Most paragraphs will work using word wrap with a single line of text in the editor, but if a single space is wanted, use two spaces at the end.
newlines make no difference in git






Hard Break:

These lines will

render exactly

two lines apart


No Break:

These lines will
render on
the same line


Soft Break:

Add two spaces AFTER each line. It will not add the extra break line.

These lines will  
render exactly  
one line apart

1. Now the list uses soft breaks for it's sub paragraphs  
 sub paragraph is lined up


####CODE:

Inline code has backticks around it

This contains `snippets` of `code` in this line

Blocks of code:
Either use three backticks on the ends of a block, or indent the block by four spaces. Only the code blocked into three backticks can contain highlights.

Syntax highlighting is not part of markdown spec, but some renderers support it

```python
This is a block of code that is indicated to be python and will inherit the properties of python code
Second line of code block
if x == 0:
    print "hello world from a code block indicated to be python"
```

```
Block of code with no indicated language.
okay. Many renderers won't know what code to render
```

    This is a block of code rendered by indent
    Block of code continued here
    The four-space style block doesn't support syntax highlighting

##TABLES

Tables are used to align columns. There must be at least 3 dashes seperating each header cell. The outer pipes are optional. The markdown does not need to line up pretty. Colons can be used in lieu of dashes at one end of the header column to specify alignment.

|Header 1| Header 2|
|--------|--------:|
| Zebra| cat|
| Monkey|Dog|

No outer|Columns
:---:|---
Centered|
large|small

Number of dashes does not matter


## Inline HTML

Simply put html within markdown

<dl>
    <dt>Definition list</dt>
    <dd>Is something people use sometimes.</dd>

    <dt>Markdown in HTML</dt>
    <dd>Does _not_ work **very** well. Use HTML <em>tags</em>.</dd>
</dl>


## Horizontal Rule

Three or more dashes

These are  

---

Rule seperated  

---
