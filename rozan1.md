
```
Node Relationships

The nodes in the node tree have relationship to each other.

The terms parent, child, and sibling are used to describe the relationships.

   -In a node tree, the top node is called the root (or root node)
   -Every node has exactly one parent, except the root (which has no parent)
   -A node can have a number of children
   -Siblings (brothers or sisters) are nodes with the same parent.
```

<html>

  <head>
      <title>DOM Tutorial</title>
  </head>

  <body>
      <h1>DOM Lesson one</h1>
      <p>Hello world!</p>
  </body>

</html>

```
From the HTML above you can read:

    <html> is the root node
    <html> has no parents
    <html> is the parent of <head> and <body>
    <head> is the first child of <html>
    <body> is the last child of <html>

and:

    <head> has one child: <title>
    <title> has one child (a text node): "DOM Tutorial"
    <body> has two children: <h1> and <p>
    <h1> has one child: "DOM Lesson one"
    <p> has one child: "Hello world!"
    <h1> and <p> are siblings
 ```
 
 <html>
<body>

<h1 id="id01">My First Page</h1>
<p id="id02"></p>

<script>
document.getElementById("id02").innerHTML = document.getElementById("id01").innerHTML;
</script>

</body>
</html>

html>
<body>

<h1 id="id01">My First Page</h1>
<p id="id02"></p>

<script>
document.getElementById("id02").innerHTML = document.getElementById("id01").firstChild.nodeValue;
</script>

</body>
</html>

