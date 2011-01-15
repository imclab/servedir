servedir
========

`servedir` is a simple [Node](http://nodejs.org) web server for offline development and testing: running `servedir` from a directory will create a quick local web server. `servedir` is useful for developing scripts that require a standard web environment and can't use the `file://` protocol.

## Installation

Check out a working copy of the source code with [Git](http://git-scm.com), or install `servedir` via [npm](http://npmjs.org). The latter will also install `servedir` into the system's `bin` path.

    $ git clone git://github.com/rem/servedir.git
    $ npm install servedir
    
Alternatively, `servedir` can be run directly from the repository using Node:

    $ node servedir.js
    
## Usage

`servedir [path] [port]`

* `path` - The location to serve files and directories from. Defaults to the current working directory.
* `port` - The port number. Default to 8000.

### Example

    $ servedir ~/Documents/example 8001
    $ servedir ~/Documents/example
    $ servedir 8001
    $ servedir
