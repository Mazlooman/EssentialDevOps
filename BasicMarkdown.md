# Markdown Guide
This is a Markdown Quick Guide. Markdown can be used for everything. People use it to create websites, documents, notes, books, presentations, email messages, and technical documentation.Markdown is portable, platform independent and everywhere. 

## Headings

|Markdown            | HTML                      | Render 
| ------------------ | ------------------------- |----------
| \# Heading level 1 | \<h1>Heading level 1\</h1>| # \# Heading level 1
 
Hint: we have 6 level header

## Table

```
| Column 1      | Column 2      |
| ------------- | ------------- |
| Cell 1, Row 1 | Cell 2, Row 1 |
| Cell 1, Row 2 | Cell 2, Row 2 |
```

## Emphasis
### Bold
|Markdown            | HTML                      | Render 
| ------------------ | ------------------------- |----------
I just love \*\*bold text\*\*.| 	I just love \<strong>bold text\</strong>. |I just love **bold text**.


### Italic
|Markdown            | HTML                      | Render 
| ------------------ | ------------------------- |----------
I just love \_italic text\_.| 	I just love \<em>Italic text\</em>. |I just love _italic text_.


### Blockquotes
To create a blockquote, add a > in front of a paragraph.
```
> Dorothy followed her through many of the beautiful rooms in her castle.
```

The rendered output looks like this:

>Dorothy followed her through many of the beautiful rooms in her castle.

## Lists
You can organize items into ordered and unordered lists.

###  Ordered Lists
```
1. First item
2. Second item
3. Third item
4. Fourth item 	 
```

### Unordered Lists
```
- First item
- Second item
- Third item
- Fourth item 
```	 
> Hint: If you need to start an unordered list item with a number followed by a period, you can use a backslash (\\) to escape the period.

## Code Blocks
### Tip 1
Code blocks are normally indented four spaces or one tab. When they’re in a list, indent them eight spaces or two tabs.

1. Open the file.
2. Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3. Update the title to match the name of your website.

### Tip 2
At the command prompt, type \`nano\`.   
rendered output:  
At the command prompt, type `nano`.

### Tip 3

```
###### JSON:
```markdown
{
    "name": "example",
    "version": "1.0.0"
}
```

Rendered Output:   
##### JSON:
```markdown
{
    "name": "example",
    "version": "1.0.0"
}
         
```

## Images

 ```
![text](/assets/images/tux.png)
```

## Links
My favorite search engine is 
```
[Duck Duck Go](https://duckduckgo.com).
```
Rendered output:  
    [Duck Duck Go](https://duckduckgo.com).


## Color
Using HTML tag
```
 <p style="color:blue">Make this text blue.</p>
```

## Comment
```
[This is a comment that will be hidden.]: # 
```

## Admonitions
```
> :warning: **Warning:** Do not push the big red button.

> :memo: **Note:** Sunrises are beautiful.

> :bulb: **Tip:** Remember to appreciate the little things in life.
```

Renderd Output:

> :warning: **Warning:** Do not push the big red button.

> :memo: **Note:** Sunrises are beautiful.

> :bulb: **Tip:** Remember to appreciate the little things in life.

## Sections
### collapsed section

```
<details>

<summary>Tips for collapsed sections</summary>

### You can add a header

You can add text within a collapsed section. 

You can add an image or a code block, too.

</details>

```
Render Output:
<details>

<summary>Tips for collapsed sections</summary>

#### You can add a header

You can add text within a collapsed section. 

You can add an image or a code block, too.

</details>

### linking section

```
[Custom foo description](#foo)
# Foo

[click on this link](#my-multi-word-header)
### My Multi Word Header
```
> Note: just one # for all heading sizes, no space between \# and anchor name, anchor tag names must be lowercase, and delimited by dashes if multi-word.

