

The Katacoda editor-terminal UI Layout combines an Editor with a Terminal. When changes are made to files using the editor, they are automatically sync'ed to the user's home directory.

# Index.json


# Helper Functionality

To support users, Katacoda has integrated various features to help users.

Copy file to editor:

var http = require('http');
var requestListener = function (req, res) {
  res.writeHead(200);
  res.end('Hello, World!');
}

var server = http.createServer(requestListener);
server.listen(3000, function() { console.log("Listening on port 3000")});

Prepend trial
<pre class="file" data-filename="app.js" data-target="prepend">console.log("Starting...")
</pre>


Append Trial
<pre class="file" data-filename="app.js" data-target="append">console.log("Finishing...")
</pre>

Add to another file trial
<pre class="file" data-filename="index.js" data-target="replace">console.log("Index.js here...")
</pre>

## New Files

Add new file

`touch newFile.js`{{execute}}

Open New File

`newFile.js`{{open}}

