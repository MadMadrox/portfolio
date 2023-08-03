# Formatting

## Table of contents

- [Headers](#headers)
- [Acceptable header names](#acceptable-header-names)
- [Collapsible content sections](#collapsible-content-sections)
- [Diagnostics](#diagnostics)
- [Bold emphasis](#bold-emphasis)
- [Code formatting](#code-formatting)
- [Error messages](#error-messages)
- [Escaping Characters](#escaping-characters)
- [Tables](#tables)
- [Lists](#lists)
- [Videos](#videos)


## Headers

Insert a blank line above and below every heading and do not include acronyms.
Spell them out in their first instance in your article.

|Header #|Formatting|Description
|:---:|:---|:---
|H1|\# Internal header|The customer does not see H1 headers. H1 is a strictly internal title.
|H2 |\#\# Customer-facing header|The customer will see H2 headers as the title of the Apollo article. The header should follow Apollo guidelines.
|H3 |\:\:\:Section Collapsible section header:\:\:<br><br>#\#\# Main section header|- H3s are used as main section headers.<br>- Both collapsible and non-collapsible count as H3, but if you are using collapsible sections, collapsible headers will be prioritized.<br>- If you're using collapsible section headers, non-collapsible headers can be used as sub-section headers inside collapsible sections.<br>- **Note**: The first collapsible section will always be automatically expanded for the reader to see. The rest will be condensed until expanded by the reader.
|H4| **\*\*Sub-section header\*\***<br>*insert a blank line here*| Sub-section header.<br>**Note**: Make sure to use two hard returned lines or the \<br\> tags after a **bold** header if you want the next line of text to start on another line. For an illustration of this issue, see the formatting example below.

**Note**: There is no H4 that is represented as: \#\#\#\#.


### Examples of header formatting

**H1-H3 formatting**

**H1-H3** will automatically set the text that follows on the next line as formatted.

For example:
>\#\#\# Section one<br>
>Here is some sample text

will render as:

>### Section one
>Here is some sample text.
<br><br>

**H4 formatting**

**H4** (when you use **bold** to format a sub-section header) ignores formatting and requires two hard returned lines afterward to recognize the text on the next line as a separate line.
- Alternatively, you can use the \<br\> tag to move text to the next line after bold headers.

For example, this text in Markdown:
>\*\*Sub-section one\*\*<br>
>Here is some sample text

will render, without the two hard returned lines, as
> **\*\*Sub-section one\*\***
>Here is some sample text

while with the two hard returned lines,

>\*\*Sub-section one\*\*<br>
>*HRL1*<br>
>*HRL2* Here is some sample text

will render correctly in Markdown as:

> **\*\*Sub-section one\*\***<br>
>Here is some sample text

Return to [Formatting: Table of contents](#table-of-contents).

## Acceptable header names
*Do not use the following headers*. They are from an outdated standard.
- Recommended steps
- Recommended documents

<br>
Acceptable, commonly used headers include:

-   Common issues and solutions

-   Troubleshooting (for unordered lists)

-   Step-by-step instructions (for ordered lists)

Return to [Formatting: Table of contents](#table-of-contents).

## Collapsible content sections

Collapsible sections can be added using the following syntax. They are useful for long articles and those with large tables, scripts, etc. 
- **Limit collapsible sections to four sections** to make the content easier to read and understand.

***Examples:***

\:\:\:Section Title of section in sentence case\:\:\:  
\* Bullet point can include links   
\* Bullet point   

\:\:\:Section Title of next section\:\:\:  
\#\#\# Can add sub section level 3 heading  
\* Subsection bullet  
\* Subsection bullet  

\#\#\# Second subsection heading  
\* Additional bullet point

Return to [Formatting: Table of contents](#table-of-contents).

## Diagnostics

For diagnostics, make the most of the features, which allow you to show
messages:

1.  While the diagnostics are running.

2.  After the diagnostic completed, but an issue wasn’t found.

***For example:***

**Instead of**:<br> We are running diagnostics.<br>
**Provide details about the diagnostics being executed**:<br> The diagnostic is running the following checks: The VM is running, RDP is enabled, firewall is opened.

**Instead of**:<br> Diagnostics completed, no issue was found.<br> 
**Provide details about the diagnostics that were executed:**<br>The diagnostic confirmed the VM is running, RDP service is enabled, and the firewall is configured correctly.

Return to [Formatting: Table of contents](#table-of-contents).

## Bold emphasis

Bold all UI elements, including buttons, blades, menus, dialogs, windows, fields, or features that have a visible name and involves user action. Don't use quotation marks or italic font in place of bold font.

**Our style**: Select the **Troubleshoot** button.<br>
**Not our style**: Select **Troubleshoot**.

- Don't overuse bold in text. 
- Use bold font occasionally, but excessive bold text can be confusing to the user, who is trying to figure out the solution. 
- In longer solutions, bold can be an effective way to make key points or issues more
scannable.
- Don't use bold for emphasis. Avoid visual emphasis of words. Build emphasis into the structure of the sentence instead. If you need to add visual emphasis, use italics.

Return to [Formatting: Table of contents](#table-of-contents).

## Code formatting

Use code formatting for code (inline and block). Other words that use code formatting are values, parameters, properties, operations, methods, functions,
language keywords, and directory and file names. Do not use code formatting on error messages.

-   For inline code, use a single backtick (\`) at the beginning and end of a code snippet.

-   For code samples and other code blocks, use three backticks (\`\`\`) on the line immediately preceding the code, and on the line immediately following the code.

-   Be sure to include a blank line after the last three backticks of a code block.
	
If you are experiencing any issues with syntax or invalid template errors for Bicep files and Azure Resource Manager templates (ARM templates), see [Resolve errors for invalid template](https://docs.microsoft.com/en-us/azure/azure-resource-manager/troubleshooting/error-invalid-template?tabs=bicep#solution-2---incorrect-segment-lengths).

Return to [Formatting: Table of contents](#table-of-contents).

## Error messages

Enclose error messages in quotation marks. Do not use backticks (\`).

***For example***:

**Our style**: If you're experiencing the "Error 999: Code not found" message, reach out to the support team.<br>
**Not our style**: If you're experiencing the `Error 999: Code not found` message, reach out to the support team.<br>
**Also not our style**: If you're experiencing the **Error 999: Code not found** message, reach out to the support team.<br>

Return to [Formatting: Table of contents](#table-of-contents).

## Escaping Characters

The need to escape characters may be necessary when you are trying to type out coding, URLs, or errors for a customer but the specific character is also used in Markdown to modify formatting. 

**Note**: These examples of escaping a character are only guaranteed to work in Elixir and GitHub. If you're working in a different client (for example, Onebranch for Azure Support Docs), the backslash may not be enough to escape characters. You may have to search for alternatives.

To display a literal character, that would otherwise be used to change the format of text in a Markdown document, add a backslash (\\) in front of the character.

***Markdown example:***

In this example, the Markdown text will look like the example below, with two backslashes before two forward slashes. 
>Input the following URL to set up your outgoing mail server: https:\\/\\/outgoing.mail.com

***Rendered example:***

By using the the back slashes, one before each of the two forward slashes, the forward slashes in the text are "escaped" and the URL will not be turned into a hyperlink. The rendered output will look like this:
>Input the following URL to set up your outgoing mail server: https:/<del></del>/outgoing.mail.com

### Characters You Can Escape

You can use a backslash to escape the following characters.

| **Character** | **Name**                                                                                                                     |
|---------------|------------------------------------------------------------------------------------------------------------------------------|
| \\            | backslash                                                                                                                    |
| \`            | backtick (see also [escaping backticks in code](https://www.markdownguide.org/basic-syntax/#escaping-backticks))             |
| \*            | asterisk                                                                                                                     |
| \_            | underscore                                                                                                                   |
| { }           | curly braces                                                                                                                 |
| [ ]           | brackets                                                                                                                     |
| \< \>         | angle brackets                                                                                                               |
| ( )           | parentheses                                                                                                                  |
| \#            | pound sign                                                                                                                   |
| +             | plus sign                                                                                                                    |
| -             | minus sign (hyphen)                                                                                                          |
| .             | dot                                                                                                                          |
| !             | exclamation mark                                                                                                             |
| \|            | pipe (see also [escaping pipe in tables](https://www.markdownguide.org/extended-syntax/#escaping-pipe-characters-in-tables)) |


## Tables

Tables are created in markdown. Use [**extended syntax**](https://www.markdownguide.org/extended-syntax/). Also, review the [**Markdown Table Generator**](https://www.tablesgenerator.com/markdown_tables).

**Note**: View your table in multiple browser types. A table that looks good in Edge might look very different in Chrome.

### Table code samples
Here are some code samples for you to copy and paste, if you need them.

**Two-column table**
```
||
|---|---
||
||
```

**Three-column table**
```
|||
|---|---|---
|||
|||

```
### Aligment of content in tables

You can align text in the columns to the left, right, or center by adding a colon `:` to the left, right, or on both sides of the hyphens within the header row (the second row of every table).

The position of the colon `:` determines the text alignment of the column.


|Alignment|Syntax|
|---|---|
| Left      |`:---`| 
| Center   |`:--:`|
| Right|`---:`|

**Example**

Here's the markdown for the table:
```
| Things | Description | More details |
| :--- | :----: | ---: |
| Thing 1 | A mediocre description | Here's more text to show that this actually aligns right |
| Thing 2 | A great description | And even more text to show that this actually aligns right |
```

And here's how it renders:

| Things | Description | More details |
|:--- |:----:|---:|
| Thing 1 | A mediocre description | Here's more text to show that this actually aligns right |
| Thing 2 | A great description | And even more text to show that this actually aligns right |


### Bulleted or numbered lists in a table

Formatting lists in tables can be a little tricky, so be sure to preview before submitting your PR.

**Note**: Currently, the \<ol\> and \<ul\> tags do not work well with Portal and causes content to be hidden if enclosed within the list tags. We recommend avoiding these tags until this issue is fixed. 

**Recommended formatting for lists in a table**

For an unordered/bulleted list:
- Use a hyphen `-` followed by a space and then your content.
- Break up each bullet and move it to the next line by using the \<br\> tag.
- Feel free to use more than one \<br\> tag if you feel that looks better.


For an ordered/numbered list:
- Use a number followed by a period `.` or right parenthesis `)` (or both), followed by a space, and then your content.
- Break up each bullet and move it to the next line by using the \<br\> tag.
- Feel free to use more than one \<br\> tag if you feel that looks better.

**Example of lists in a table**

Here's the Markdown formatting of lists in a table:

```
| Type of list | Description | Here's the list |
| :--- | :--- | :--- |
| Unordered list | A description |- bullet one <br>- bullet two<br>- bullet three |
| Ordered list| A description |1. bullet one <br>2. bullet two<br>3. bullet three |
```

Here's how it renders:

| Type of list | Description | Here's the list |
|:---|:---|:---|
| Unordered list | A description |- bullet one <br>- bullet two<br>- bullet three |
| Ordered list| A description |1. bullet one <br>2. bullet two<br>3. bullet three |


<!-- Commenting this out because ol/ul tags do not currently play nice with Portal, and when and if they do at some point in the future, we don't want to have to retype all of this

**Note**: Do not use any hard returns/line breaks/carriage returns when formatting a list within a table. Using the **\<ol\>**, **\<ul\>**, **\<li\>** tags properly will automate line breaks between each bullet point. Outside of the lists, use the **\<br\>** tag to create your line breaks. Any hard line breaks will break the table structure.

1.  **\<br\> tags**: This is the simplest way to create a “list” in a table. There
    won’t be numbers or bullets, but you can separate items in a list by using
    two break tags to create space (\<br\>\<br\>).

2.  **Ordered lists**: This creates a numbered list.

	>\<ol\>\<li\>first item\</li\>\<li\>second item\</li\>\<li\>third item\</li\>\</ol\>

	-   Don’t add spaces before, after, or between the tags \<ol\>\<li\>, \</li\>\<li\>, and \</li\>\</ol\>.

	-   You can still use \<br\> tags.

3.  **Unordered lists**: This creates a bulleted list.

	>\<ul\>\<li\>first item\</li\>\<li\>second item\</li\>\<li\>third item\</li\>\</ul\>

	-   Don’t add spaces before, after, or between the tags \<ul\>\<li\>, \</li\>\<li\>, and \</li\>\</ul\>.

	-   You can still use \<br\> tags.
-->

### Maximum column or row limit for tables

-   Max columns = 10

-   Max rows = 1,000

Return to [Formatting: Table of contents](#table-of-contents).

## Lists

There are two types of lists you can use in Markdown.
- Unordered/bulleted list
- Ordered/numbered list

### Unordered list
An unordered/bulleted list uses either an asterisk `*`, hyphen `-` or plus `+` to create an unordered list.

Here's an example of an unordered list using Markdown:
```
* item 1
* Item 2
- Item 3
- Item 4
+ item 5
+ item 6
```

And here's how it will render:
- item 1
- Item 2
- Item 3
- Item 4
- item 5
- item 6

### Ordered list
An ordered/numbered list uses a number followed by a period `.` or right parentheses `)` to create an ordered list.
- It doesn't matter if you number your list in ascending order, the numbers will automatically adjust in order. For example, if you only have a short list with no breaks in the list, you can number each entry with a 1 and the numbers will automatically be generated in order. See **Example 2**.
- It *does matter* which number you start with. The numbers will continue and count down from the first number in your list. This is beneficial for numbered lists you wish to continue after a break in the list. See **Example 3**.
- If there is a break in your numbered list (for example, you insert a **Note**, image, or extra content in between entries), and you wish to continue your previous numbered list, start the new numbered list with the next logical number in the list. Once the numbered list is contained without a break, the numbering doesn't matter again. The numbers will be automatically generated in order. See **Example 3**.

**Example 1: Standard ordered list numbering**

Here's an example of an ordered list using Markdown:
```
1. step 1
2. step 2
3. step 3
4. step 4
5. step 5
6. step 6
```

And here's how it will render:
1. step 1
2. step 2
3. step 3
4. step 4
5. step 5
6. step 6

**Example 2: Using the same number for each bullet**

Here's an example of an ordered list in Markdown using the same number for each entry.
```
1. step 1
1. step 2
1. step 3
1. step 4
1. step 5
1. step 6
```

This example will still render as:
1. step 1
1. step 2
1. step 3
1. step 4
1. step 5
1. step 6

**Example 3: Continuing the ordered list after a break**

Here's an example of continuing the ordered list in Markdown after a break in the list.
```
1. step 1
1. step 2
1. step 3

[There is a break in the list here.]

4. step 4
4. step 5
4. step 6
```

This example will render as:
1. step 1
1. step 2
1. step 3

`[There is a break in the list here.]`

4. step 4
4. step 5
4. step 6

<!-- This does not seem to render on the website...
### Task lists
To create a task list, use a hyphen `-` followed by a space, followed by \[ \]. To mark a task as complete, use \[x\].
```
- [x] Wash the dishes
- [ ] Take out the trash
- [ ] Say a little prayer for me
```

Here's how it renders:
- [x] Wash the dishes
- [ ] Take out the trash
- [ ] Say a little prayer for me
-->

Return to [Formatting: Table of contents](#table-of-contents).

## Videos

To meet accessibility standards, include a brief introduction that describes how the video helps resolve the issue.

**Note:** When using YouTube links, avoid the ampersand character (&). This character prevents the video from rendering correctly.

**Example**: 
>The following video shows how to register an application through
the App registration experience. Steps include adding a client secret, adding an
owner to the application, and API permissions to get the application data using
Microsoft Graph.   

<br>If it’s a long video (more than 3 minutes), consider calling out the highlights
of the video with timestamps.

**Example**: 
>At 1:25, learn how to add a client secret. At 3:30, learn how to
add an owner to the application.

<br>**Note**: Videos must be sourced from YouTube. Videos with a short URL, such as youtu.be,
or videos with a timestamp, are not currently supported. Replace the CAPITALIZED
TEXT in the following schema with specifics.

<br>**One video**

Use the following schema for one video. 
- Make sure there is a blank line after any preceding content, before the opening `<video>` tag, and after the closing `</video>` tag.

		*blank line*
		<video>
			<src>https://www.youtube.com/sampleURL</src>
			<title>**VIDEO TITLE EXAMPLE: How to use Azure Bastion to securely**</title>
		</video>
		*blank line*

<br>**More than one video**

Use the following schema for more than one video. 
- This only works for groups of videos up to a maximum of three. 
- Make sure there is a blank line after any preceding content, before the opening `<videoGroup>` tag, and after the closing `</videoGroup>` tag.

		*blank line*
		<videoGroup>
			<video>
				<src>https://www.youtube.com/sampleURL01</src>
				<title>**VIDEO TITLE EXAMPLE: Connecting to GitHub**</title>
			</video>
			<video>
				<src>https://www.youtube.com/sampleURL02</src>
				<title>**VIDEO TITLE EXAMPLE: Connecting to SalesForce**</title>
			</video>
			<video>
				<src>https://www.youtube.com/sampleURL03</src>
				<title>**VIDEO TITLE EXAMPLE: Connecting to Slack**</title>
			</video>
		</videoGroup>
		*blank line*


Return to [Formatting: Table of contents](#table-of-contents).
