# gitbook-plugin-flowchart

[![NPM](https://nodei.co/npm/gitbook-plugin-flowchart.png)](https://nodei.co/npm/gitbook-plugin-flowchart/)

[flowchart.js](https://github.com/adrai/flowchart.js) plugin for [GitBook](https://github.com/GitbookIO/gitbook)

## Installation

    $ npm install gitbook-plugin-flowchart

book.json add the plugin

```
{
  "plugins": ["flowchart"]
}
```

## Configuration

book.json add the flowchart.js options

```
"pluginsConfig": {
  "flowchart": {
    "line-color": "red"
  }
}
```

## Usage

put in your book block as

```
{% flowchart %}
st=>start: Start:>http://www.google.com[blank]
e=>end:>http://www.google.com
op1=>operation: My Operation
sub1=>subroutine: My Subroutine
cond=>condition: Yes
or No?:>http://www.google.com
io=>inputoutput: catch something...

st->op1->cond
cond(yes)->io->e
cond(no)->sub1(right)->op1
{% endflowchart %}
```

### Extend the width

```
{% flowchart width=770 %}
```
