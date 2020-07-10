---
title : "Markdown Cheat Sheet"
date: 2020-07-09T11:14:04+05:30
tags: 
  - Markdown
---


# Markdown Cheat Sheet

Thanks for visiting [The Markdown Guide](https://www.markdownguide.org)!

This Markdown cheat sheet provides a quick overview of all the Markdown syntax elements. It can’t cover every edge case, so if you need more information about any of these elements, refer to the reference guides for [basic syntax](https://www.markdownguide.org/basic-syntax) and [extended syntax](https://www.markdownguide.org/extended-syntax).

## Basic Syntax

These are the elements outlined in John Gruber’s original design document. All Markdown applications support these elements.

```
# H1
## H2
### H3

### Bold
**bold text**
```


### Heading

# H1
## H2
### H3

### Bold

**bold text**

```
### Italic
```
### Italic

*italicized text*
```
### Blockquote
```

### Blockquote

> blockquote


```
### Ordered List

1. First item
2. Second item
3. Third item

### Unordered List

- First item
- Second item
- Third item
```

### Ordered List

1. First item
2. Second item
3. Third item

### Unordered List

- First item
- Second item
- Third item

### Code

```
`code`

```

`code`

### Horizontal Rule
```
---
```

---

### Link

[title](https://www.example.com)

### Image
```
![alt text](/images/img.jpg)
```

![alt text](/images/img.jpg)

## Extended Syntax

These elements extend the basic syntax by adding additional features. Not all Markdown applications support these elements.

### Table

```
| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |
```


| Syntax | Description |
| ----------- | ----------- |
| Header | Title |
| Paragraph | Text |

### Fenced Code Block

```
{
  "firstName": "John",
  "lastName": "Smith",
  "age": 25
}
```

### Footnote

Here's a sentence with a footnote. [^1]

[^1]: This is the footnote.

### Heading ID

### My Great Heading {#custom-id}

### Definition List

```
term
: definition
```

term
: definition

### Strikethrough
```
~~The world is flat.~~
```

~~The world is flat.~~

### Task List
```
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

```

- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media



### UPDATE

To add Code snippets, you can use 

```

{{ < highlight javascript > }} (Dont leave spaces between brackets and the less/greater signs)
//  OpenShift sample Node application
var express = require('express'),
    fs      = require('fs'),
    app     = express(),
    eps     = require('ejs'),
    morgan  = require('morgan');
    
Object.assign=require('object-assign')

app.engine('html', require('ejs').renderFile);
app.use(morgan('combined'))

var port = process.env.PORT || process.env.OPENSHIFT_NODEJS_PORT || 8080,
    ip   = process.env.IP   || process.env.OPENSHIFT_NODEJS_IP || '0.0.0.0',
    mongoURL = process.env.OPENSHIFT_MONGODB_DB_URL || process.env.MONGO_URL,
    mongoURLLabel = "";
{{ < /highlight > }} (Dont leave spaces between brackets and the less/greater signs)


```
RESULT

{{< highlight javascript >}}
//  OpenShift sample Node application
var express = require('express'),
    fs      = require('fs'),
    app     = express(),
    eps     = require('ejs'),
    morgan  = require('morgan');
    
Object.assign=require('object-assign')

app.engine('html', require('ejs').renderFile);
app.use(morgan('combined'))

var port = process.env.PORT || process.env.OPENSHIFT_NODEJS_PORT || 8080,
    ip   = process.env.IP   || process.env.OPENSHIFT_NODEJS_IP || '0.0.0.0',
    mongoURL = process.env.OPENSHIFT_MONGODB_DB_URL || process.env.MONGO_URL,
    mongoURLLabel = "";
{{< /highlight >}}


To show git gist use
```
{{  < gist dischord01 f43dbb1b2cdfc4c3802f  >  }} (Dont leave spaces between brackets and the less/greater signs)

```
RESULT

{{< gist dischord01 f43dbb1b2cdfc4c3802f  >}}