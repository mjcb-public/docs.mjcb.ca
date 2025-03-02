---
title: "Markdown Cheatsheet"
geekdocNav: true
geekdocAnchor: false
---

{{< hint type=note title="Markdown Content" >}}
This is a basic [Markdown](https://commonmark.org/) cheatsheet. It does not include every possible markdown option, as those can vary depending on what platform is used. This cheatsheet mostly applies to [Hugo](https://gohugo.io/).
{{< /hint >}}

* [Headings](#headings)
    * [Custom Heading ID](#custom-heading-id)
* [Horizontal Rule](#horizontal-rule)
* [Text](#text)
    * [Bold](#bold)
    * [Italics](#italics)
    * [Bold and Italics](#bold-and-italics)
    * [Strikethrough](#strikethrough)
* [Lists](#lists)
    * [Ordered List](#ordered-list)
    * [Unordered List](#unordered-list)
    * [Task List](#task-list)
    * [Nested Lists](#nested-lists)
    * [Definition Lists](#definition-lists)
* [Code](#code)
    * [Blockquotes](#blockquotes)
    * [Inline Code](#inline-code)
    * [Fenced Code Block](#fenced-code-block)
* [Tables](#tables)
* [Footnotes](#footnotes)
* [Images](#images)
* [Links](#links)

## Headings ##

Headings can have the `#` character after the header text and it will render the same:

```
# Heading Level 1

## Heading Level 2 ##

### Heading Level 3

#### Heading Level 4 ####

##### Heading Level 5

###### Heading Level 6
```

# Heading Level 1

## Heading Level 2 ##

### Heading Level 3

#### Heading Level 4 ####

##### Heading Level 5

###### Heading Level 6

### Custom Heading ID ###

Markdown also supports customizing the heading ID should that be required:

```
# Custom Heading {#custom-heading-id}
```

## Horizontal Rule ##

A horizontal rule can be inserted by having three or more `-`, `+` or `_` characters in a row by themselves:

```
---
```

---

## Text ##

### Bold ###

Bold text can be inserted with two `*` or `_` characters on each side of the text to be bolded:

```
**Bold text**
```

**Bold text**

### Italics ###

Italicized text can be inserted with one `*` or `_` characters on each side of the text to be italicized:

```
*Italics text*
```

*Italics text*

### Bold and Italics ###

Text can be bolded and italicized with three `*` or `_` characters on each side of the text to be highlighted:

```
**Bold and italics text**
```

***Bold and italics text***

### Strikethrough ###

To strikethrough text, insert two `~` characters on each side of the text:

```
~~Strikethrough text~~
```

~~Strikethrough text~~

## Lists ##

### Ordered List ###

Ordered lists work just like a regular ordered list in HTML:

```
1. Ordered list item one.
2. Ordered list item two.
3. Ordered list item three.
```

1. Ordered list item one.
2. Ordered list item two.
3. Ordered list item three.

### Unordered List ###

Unordered lists work just like regular unordered lists in HTML:

```
* Unordered list item one.
* Unordered list item two.
* Unordered list item three.
```

* Unordered list item one.
* Unordered list item two.
* Unordered list item three.

The list can use the `-`, `*`, or `+` characters.

### Task List ###

Tasks lists can be added list a normal list with the `[ ]` characters to represent an unchecked box, and `[X]` characters representing a checked box:

```
- [x] Task list item one.
- [ ] Task list item two.
- [ ] Task list item three.
```

- [x] Task list item one.
- [ ] Task list item two.
- [ ] Task list item three.

### Nested Lists ###

Nested lists can be created by inserting four spaces before the list item:

```
* Unordered list item one.
    * Unordered nested list item one.
    * Unordered nested list item two.
    * Unordered nested list item three.
* Unordered list item two.
* Unordered list item three.
```

* Unordered list item one.
    * Unordered nested list item one.
    * Unordered nested list item two.
    * Unordered nested list item three.
* Unordered list item two.
* Unordered list item three.

It can also be mixed with ordered lists as well:

```
1. Unordered list item one.
    * Unordered nested list item one.
    * Unordered nested list item two.
    * Unordered nested list item three.
2. Unordered list item two.
3. Unordered list item three.
```

1. Unordered list item one.
    * Unordered nested list item one.
    * Unordered nested list item two.
    * Unordered nested list item three.
2. Unordered list item two.
3. Unordered list item three.

### Definition Lists ###

Definition lists can be created by using the `:` character on a separate line after the header:

```
Term One
: Definition One

Term Two
: Definition Two

Term Three
: Definition Three
```

Term One
: Definition One

Term Two
: Definition Two

Term Three
: Definition Three

Ensure that there is a blank line between list items if there are multiple items.

## Code ##

### Blockquotes ###

Blockquotes can be created by using the `>` character:

```
> Blockquote
```

> Blockquote

### Inline Code ###

Code items can be inserted inline for reference purposes:

```
A `code sample` can be inserted into a sentence.
```

A `code sample` can be inserted into a sentence.

### Fenced Code Block ###

Larger blocks of code can be used by wrapping the content in three backtick characters at the beginning and the end:

````
```
<?php
    echo "Hello world";
?>
```
````

```
<?php
    echo "Hello world";
?>
```

Markdown also offers syntax highlighting depending on which version is being used. Hugo [supports](https://gohugo.io/content-management/syntax-highlighting/#list-of-chroma-highlighting-languages) several languages. In this example, PHP syntax highlighting is used:

```php
<?php
    echo "Hello world";
?>
```

### Tables ###

Tables can be inserted by using a `|` to represent the columns and at least three `---` characters to create the header for the table:

```
| Cell | Cell | Cell |
|------|------|------|
| Cell | Cell | Cell |
| Cell | Cell | Cell |
| Cell | Cell | Cell |
```

| Cell | Cell | Cell |
|------|------|------|
| Cell | Cell | Cell |
| Cell | Cell | Cell |
| Cell | Cell | Cell |

The cells in the table can be aligned by using a `:` character on the header to set the alignment for the column:

```
| Cell | Cell   | Cell  |
|:-----|:------:|------:|
| Left | Center | Right |
| Left | Center | Right |
| Left | Center | Right |
```

| Cell | Cell   | Cell  |
|:-----|:------:|------:|
| Left | Center | Right |
| Left | Center | Right |
| Left | Center | Right |

### Footnotes ###

Footnotes can be created by inserting the reference point (`[^1]`) for the footnote and then inserting the content with the same reference:

```
This sentence has a footnote that is referenced at the end of the page.[^1]

[^1]: This is the footnote that was referenced.
```

This sentence has a footnote that is referenced at the end of the page.[^1]

[^1]: This is the footnote that was referenced.

### Links ###

To create a link in Markdown, enclose the link name in brackets (`[]`) and then immediately with the URL in parentheses (`()`):

```
[mjcb.ca](https://mjcb.ca/)
```

[mjcb.ca](https://mjcb.ca/)

Link titles can also be added within the parentheses if required:

```
[mjcb.ca](https://mjcb.ca/ "mjcb.ca Homepage")
```

[mjcb.ca](https://mjcb.ca/ "mjcb.ca Homepage")

Links and email addresses can also be quickly created by enclosing a URL or email address in angle brackets `<>`:

```
<https://mjcb.ca/>

<matthew@docs.mjcb.ca>
```

<https://mjcb.ca/>

<matthew@docs.mjcb.ca>

### Images ###

Images can be created by adding the alternate text and the image path in text brackets and parentheses starting with an exclamation point `![]()`:

```
![docs.mjcb.ca Alt Text](/images/miscellaneous/markdown/markdown-cheatsheet/docs.png)
```

![docs.mjcb.ca Alt Text](/images/miscellaneous/markdown/markdown-cheatsheet/docs.png)

Optionally, a title for the image can be added with the path of the image:

```
![docs.mjcb.ca Alt Text](/images/miscellaneous/markdown/markdown-cheatsheet/docs.png "docs.mjcb.ca Title")
```
