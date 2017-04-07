# api documentation for  [union (v0.4.6)](https://github.com/flatiron/union#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-union.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-union) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-union.svg)](https://travis-ci.org/npmdoc/node-npmdoc-union)
#### A hybrid buffered / streaming middleware kernel backwards compatible with connect.

[![NPM](https://nodei.co/npm/union.png?downloads=true)](https://www.npmjs.com/package/union)

[![apidoc](https://npmdoc.github.io/node-npmdoc-union/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-union_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-union/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-union/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-union/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Charlie Robbins",
        "email": "charlie.robbins@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/flatiron/union/issues"
    },
    "dependencies": {
        "qs": "~2.3.3"
    },
    "description": "A hybrid buffered / streaming middleware kernel backwards compatible with connect.",
    "devDependencies": {
        "connect": "2.22.x",
        "director": "1.x.x",
        "ecstatic": "0.5.x",
        "request": "2.29.x",
        "vows": "0.8.0"
    },
    "directories": {},
    "dist": {
        "shasum": "198fbdaeba254e788b0efcb630bc11f24a2959e0",
        "tarball": "https://registry.npmjs.org/union/-/union-0.4.6.tgz"
    },
    "engines": {
        "node": ">= 0.8.0"
    },
    "gitHead": "0dfda9acdec355997b09c4b85e2906cb4b46014f",
    "homepage": "https://github.com/flatiron/union#readme",
    "main": "./lib",
    "maintainers": [
        {
            "name": "indexzero",
            "email": "charlie.robbins@gmail.com"
        },
        {
            "name": "dscape",
            "email": "nunojobpinto@gmail.com"
        },
        {
            "name": "jcrugzz",
            "email": "jcrugzz@gmail.com"
        },
        {
            "name": "swaagie",
            "email": "info@martijnswaagman.nl"
        }
    ],
    "name": "union",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/flatiron/union.git"
    },
    "scripts": {
        "test": "vows test/*-test.js --spec -i"
    },
    "version": "0.4.6"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module union](#apidoc.module.union)
1.  [function <span class="apidocSignatureSpan">union.</span>BufferedStream (limit)](#apidoc.element.union.BufferedStream)
1.  [function <span class="apidocSignatureSpan">union.</span>HttpStream (options)](#apidoc.element.union.HttpStream)
1.  [function <span class="apidocSignatureSpan">union.</span>ResponseStream (options)](#apidoc.element.union.ResponseStream)
1.  [function <span class="apidocSignatureSpan">union.</span>RoutingStream (options)](#apidoc.element.union.RoutingStream)
1.  [function <span class="apidocSignatureSpan">union.</span>RoutingStream.super_ (options)](#apidoc.element.union.RoutingStream.super_)
1.  [function <span class="apidocSignatureSpan">union.</span>createServer (options)](#apidoc.element.union.createServer)
1.  [function <span class="apidocSignatureSpan">union.</span>errorHandler (err, req, res)](#apidoc.element.union.errorHandler)
1.  object <span class="apidocSignatureSpan">union.</span>BufferedStream.prototype
1.  object <span class="apidocSignatureSpan">union.</span>HttpStream.prototype
1.  object <span class="apidocSignatureSpan">union.</span>ResponseStream.prototype
1.  object <span class="apidocSignatureSpan">union.</span>RoutingStream.prototype
1.  object <span class="apidocSignatureSpan">union.</span>RoutingStream.super_.prototype
1.  object <span class="apidocSignatureSpan">union.</span>core
1.  string <span class="apidocSignatureSpan">union.</span>version

#### [module union.BufferedStream](#apidoc.module.union.BufferedStream)
1.  [function <span class="apidocSignatureSpan">union.</span>BufferedStream (limit)](#apidoc.element.union.BufferedStream.BufferedStream)
1.  [function <span class="apidocSignatureSpan">union.BufferedStream.</span>super_ ()](#apidoc.element.union.BufferedStream.super_)

#### [module union.BufferedStream.prototype](#apidoc.module.union.BufferedStream.prototype)
1.  [function <span class="apidocSignatureSpan">union.BufferedStream.prototype.</span>close ()](#apidoc.element.union.BufferedStream.prototype.close)
1.  [function <span class="apidocSignatureSpan">union.BufferedStream.prototype.</span>destroy ()](#apidoc.element.union.BufferedStream.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">union.BufferedStream.prototype.</span>end ()](#apidoc.element.union.BufferedStream.prototype.end)
1.  [function <span class="apidocSignatureSpan">union.BufferedStream.prototype.</span>pause ()](#apidoc.element.union.BufferedStream.prototype.pause)
1.  [function <span class="apidocSignatureSpan">union.BufferedStream.prototype.</span>pipe ()](#apidoc.element.union.BufferedStream.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">union.BufferedStream.prototype.</span>resume ()](#apidoc.element.union.BufferedStream.prototype.resume)
1.  [function <span class="apidocSignatureSpan">union.BufferedStream.prototype.</span>write (chunk)](#apidoc.element.union.BufferedStream.prototype.write)

#### [module union.HttpStream](#apidoc.module.union.HttpStream)
1.  [function <span class="apidocSignatureSpan">union.</span>HttpStream (options)](#apidoc.element.union.HttpStream.HttpStream)
1.  [function <span class="apidocSignatureSpan">union.HttpStream.</span>super_ (limit)](#apidoc.element.union.HttpStream.super_)

#### [module union.HttpStream.prototype](#apidoc.module.union.HttpStream.prototype)
1.  [function <span class="apidocSignatureSpan">union.HttpStream.prototype.</span>pipeState (source)](#apidoc.element.union.HttpStream.prototype.pipeState)

#### [module union.ResponseStream](#apidoc.module.union.ResponseStream)
1.  [function <span class="apidocSignatureSpan">union.</span>ResponseStream (options)](#apidoc.element.union.ResponseStream.ResponseStream)
1.  [function <span class="apidocSignatureSpan">union.ResponseStream.</span>super_ (options)](#apidoc.element.union.ResponseStream.super_)

#### [module union.ResponseStream.prototype](#apidoc.module.union.ResponseStream.prototype)
1.  [function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>_implicitHeader ()](#apidoc.element.union.ResponseStream.prototype._implicitHeader)
1.  [function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>addTrailers ()](#apidoc.element.union.ResponseStream.prototype.addTrailers)
1.  [function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>end (data)](#apidoc.element.union.ResponseStream.prototype.end)
1.  [function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>getHeader ()](#apidoc.element.union.ResponseStream.prototype.getHeader)
1.  [function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>html (str)](#apidoc.element.union.ResponseStream.prototype.html)
1.  [function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>json (obj)](#apidoc.element.union.ResponseStream.prototype.json)
1.  [function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>pipe ()](#apidoc.element.union.ResponseStream.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>redirect (path, status)](#apidoc.element.union.ResponseStream.prototype.redirect)
1.  [function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>removeHeader ()](#apidoc.element.union.ResponseStream.prototype.removeHeader)
1.  [function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>setHeader ()](#apidoc.element.union.ResponseStream.prototype.setHeader)
1.  [function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>text (str)](#apidoc.element.union.ResponseStream.prototype.text)
1.  [function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>write (data)](#apidoc.element.union.ResponseStream.prototype.write)
1.  [function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>writeHead (statusCode, statusMessage, headers)](#apidoc.element.union.ResponseStream.prototype.writeHead)

#### [module union.RoutingStream](#apidoc.module.union.RoutingStream)
1.  [function <span class="apidocSignatureSpan">union.</span>RoutingStream (options)](#apidoc.element.union.RoutingStream.RoutingStream)
1.  [function <span class="apidocSignatureSpan">union.RoutingStream.</span>super_ (options)](#apidoc.element.union.RoutingStream.super_)

#### [module union.RoutingStream.prototype](#apidoc.module.union.RoutingStream.prototype)
1.  [function <span class="apidocSignatureSpan">union.RoutingStream.prototype.</span>onError (err)](#apidoc.element.union.RoutingStream.prototype.onError)
1.  [function <span class="apidocSignatureSpan">union.RoutingStream.prototype.</span>route (req)](#apidoc.element.union.RoutingStream.prototype.route)

#### [module union.RoutingStream.super_](#apidoc.module.union.RoutingStream.super_)
1.  [function <span class="apidocSignatureSpan">union.RoutingStream.</span>super_ (options)](#apidoc.element.union.RoutingStream.super_.super_)

#### [module union.RoutingStream.super_.prototype](#apidoc.module.union.RoutingStream.super_.prototype)
1.  [function <span class="apidocSignatureSpan">union.RoutingStream.super_.prototype.</span>pipeRequest (source)](#apidoc.element.union.RoutingStream.super_.prototype.pipeRequest)
1.  [function <span class="apidocSignatureSpan">union.RoutingStream.super_.prototype.</span>setEncoding ()](#apidoc.element.union.RoutingStream.super_.prototype.setEncoding)

#### [module union.core](#apidoc.module.union.core)
1.  [function <span class="apidocSignatureSpan">union.core.</span>createServer (options)](#apidoc.element.union.core.createServer)
1.  [function <span class="apidocSignatureSpan">union.core.</span>errorHandler (err, req, res)](#apidoc.element.union.core.errorHandler)



# <a name="apidoc.module.union"></a>[module union](#apidoc.module.union)

#### <a name="apidoc.element.union.BufferedStream"></a>[function <span class="apidocSignatureSpan">union.</span>BufferedStream (limit)](#apidoc.element.union.BufferedStream)
- description and source-code
```javascript
BufferedStream = function (limit) {
  events.EventEmitter.call(this);

  if (typeof limit === 'undefined') {
    limit = Infinity;
  }

  this.limit = limit;
  this.size = 0;
  this.chunks = [];
  this.writable = true;
  this.readable = true;
  this._buffer = true;
}
```
- example usage
```shell
...
  @param limit {Number}
  the limit for which the stream can be buffered
'''

Example

'''js
var bs = union.BufferedStream(n);
'''

## HttpStream Constructor
This constructor inherits from 'union.BufferedStream' and returns a stream with these extra properties:

Specification
...
```

#### <a name="apidoc.element.union.HttpStream"></a>[function <span class="apidocSignatureSpan">union.</span>HttpStream (options)](#apidoc.element.union.HttpStream)
- description and source-code
```javascript
HttpStream = function (options) {
  options = options || {};
  BufferedStream.call(this, options.limit);

  if (options.buffer === false) {
    this.buffer = false;
  }

  this.on('pipe', this.pipeState);
}
```
- example usage
```shell
...
'''
  function HttpStream()
'''

Example

'''js
var hs = union.HttpStream();
'''

## HttpStream Instance Members

### url
The url from the request.
...
```

#### <a name="apidoc.element.union.ResponseStream"></a>[function <span class="apidocSignatureSpan">union.</span>ResponseStream (options)](#apidoc.element.union.ResponseStream)
- description and source-code
```javascript
ResponseStream = function (options) {
  var self = this,
      key;

  options = options || {};
  HttpStream.call(this, options);

  this.writeable = true;
  this.response = options.response;

  if (options.headers) {
    for (key in options.headers) {
      this.response.setHeader(key, options.headers[key]);
    }
  }

  //
  // Proxy 'statusCode' changes to the actual 'response.statusCode'.
  //
  Object.defineProperty(this, 'statusCode', {
    get: function () {
      return self.response.statusCode;
    },
    set: function (value) {
      self.response.statusCode = value;
    },
    enumerable: true,
    configurable: true
  });

  if (this.response) {
    this._headers = this.response._headers = this.response._headers || {};

    // Patch to node core
    this.response._headerNames = this.response._headerNames || {};

    //
    // Proxy to emit "header" event
    //
    this._renderHeaders = this.response._renderHeaders;
    this.response._renderHeaders = function () {
      if (!self._emittedHeader) {
        self._emittedHeader = true;
        self.headerSent = true;
        self._header = true;
        self.emit('header');
      }

      return self._renderHeaders.call(self.response);
    };
  }
}
```
- example usage
```shell
...
'''
  function ResponseStream()
'''

Example

'''js
var rs = union.ResponseStream();
'''

# Tests

All tests are written with [vows][0] and should be run with [npm][1]:

''' bash
...
```

#### <a name="apidoc.element.union.RoutingStream"></a>[function <span class="apidocSignatureSpan">union.</span>RoutingStream (options)](#apidoc.element.union.RoutingStream)
- description and source-code
```javascript
RoutingStream = function (options) {
  options = options || {};
  RequestStream.call(this, options);

  this.before = options.before || [];
  this.after = options.after || [];
  this.response = options.response || options.res;
  this.headers = options.headers || {
    'x-powered-by': 'union ' + union.version
  };

  this.target = new ResponseStream({
    response: this.response,
    headers: this.headers
  });

  this.once('pipe', this.route);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.RoutingStream.super_"></a>[function <span class="apidocSignatureSpan">union.</span>RoutingStream.super_ (options)](#apidoc.element.union.RoutingStream.super_)
- description and source-code
```javascript
RoutingStream.super_ = function (options) {
  options = options || {};
  HttpStream.call(this, options);

  this.on('pipe', this.pipeRequest);
  this.request = options.request;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.createServer"></a>[function <span class="apidocSignatureSpan">union.</span>createServer (options)](#apidoc.element.union.createServer)
- description and source-code
```javascript
createServer = function (options) {
  var isArray = Array.isArray(options.after),
      credentials;

  if (!options) {
    throw new Error('options is required to create a server');
  }

  function requestHandler(req, res) {
    var routingStream = new RoutingStream({
      before: options.before,
      buffer: options.buffer,
      //
      // Remark: without new after is a huge memory leak that
      // pipes to every single open connection
      //
      after: isArray && options.after.map(function (After) {
        return new After;
      }),
      request: req,
      response: res,
      limit: options.limit,
      headers: options.headers
    });

    routingStream.on('error', function (err) {
      var fn = options.onError || core.errorHandler;
      fn(err, routingStream, routingStream.target, function () {
        routingStream.target.emit('next');
      });
    });

    req.pipe(routingStream);
  }

  //
  // both https and spdy requires same params
  //
  if (options.https || options.spdy) {
    if (options.https && options.spdy) {
      throw new Error('You shouldn\'t be using https and spdy simultaneously.');
    }

    var serverOptions,
        credentials,
        key = !options.spdy
          ? 'https'
          : 'spdy';

    serverOptions = options[key];
    if (!serverOptions.key || !serverOptions.cert) {
      throw new Error('Both options.' + key + '.'key' and options.' + key + '.'cert' are required.');
    }

    credentials = {
      key:  fs.readFileSync(serverOptions.key),
      cert: fs.readFileSync(serverOptions.cert)
    };

    if (serverOptions.ca) {
      serverOptions.ca = !Array.isArray(serverOptions.ca)
        ? [serverOptions.ca]
        : serverOptions.ca

      credentials.ca = serverOptions.ca.map(function (ca) {
        return fs.readFileSync(ca);
      });
    }

    if (options.spdy) {
      // spdy is optional so we require module here rather than on top
      var spdy = require('spdy');
      return spdy.createServer(credentials, requestHandler);
    }

    return https.createServer(credentials, requestHandler);
  }

  return http.createServer(requestHandler);
}
```
- example usage
```shell
...
''' js
var fs = require('fs'),
  union = require('../lib'),
  director = require('director');

var router = new director.http.Router();

var server = union.createServer({
before: [
  function (req, res) {
    var found = router.dispatch(req, res);
    if (!found) {
      res.emit('next');
    }
  }
...
```

#### <a name="apidoc.element.union.errorHandler"></a>[function <span class="apidocSignatureSpan">union.</span>errorHandler (err, req, res)](#apidoc.element.union.errorHandler)
- description and source-code
```javascript
function error(err, req, res) {
  if (err) {
    (this.res || res).writeHead(err.status || 500, err.headers || { "Content-Type": "text/plain" });
    (this.res || res).end(err.message + "\n");
    return;
  }

  (this.res || res).writeHead(404, {"Content-Type": "text/plain"});
  (this.res || res).end("Not Found\n");
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.union.BufferedStream"></a>[module union.BufferedStream](#apidoc.module.union.BufferedStream)

#### <a name="apidoc.element.union.BufferedStream.BufferedStream"></a>[function <span class="apidocSignatureSpan">union.</span>BufferedStream (limit)](#apidoc.element.union.BufferedStream.BufferedStream)
- description and source-code
```javascript
BufferedStream = function (limit) {
  events.EventEmitter.call(this);

  if (typeof limit === 'undefined') {
    limit = Infinity;
  }

  this.limit = limit;
  this.size = 0;
  this.chunks = [];
  this.writable = true;
  this.readable = true;
  this._buffer = true;
}
```
- example usage
```shell
...
  @param limit {Number}
  the limit for which the stream can be buffered
'''

Example

'''js
var bs = union.BufferedStream(n);
'''

## HttpStream Constructor
This constructor inherits from 'union.BufferedStream' and returns a stream with these extra properties:

Specification
...
```

#### <a name="apidoc.element.union.BufferedStream.super_"></a>[function <span class="apidocSignatureSpan">union.BufferedStream.</span>super_ ()](#apidoc.element.union.BufferedStream.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.union.BufferedStream.prototype"></a>[module union.BufferedStream.prototype](#apidoc.module.union.BufferedStream.prototype)

#### <a name="apidoc.element.union.BufferedStream.prototype.close"></a>[function <span class="apidocSignatureSpan">union.BufferedStream.prototype.</span>close ()](#apidoc.element.union.BufferedStream.prototype.close)
- description and source-code
```javascript
close = function () {
  this.readable = false;
  this.closed = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.BufferedStream.prototype.destroy"></a>[function <span class="apidocSignatureSpan">union.BufferedStream.prototype.</span>destroy ()](#apidoc.element.union.BufferedStream.prototype.destroy)
- description and source-code
```javascript
destroy = function () {
  this.readable = false;
  this.writable = false;
  delete this.chunks;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.BufferedStream.prototype.end"></a>[function <span class="apidocSignatureSpan">union.BufferedStream.prototype.</span>end ()](#apidoc.element.union.BufferedStream.prototype.end)
- description and source-code
```javascript
end = function () {
  this.readable = false;
  this.ended = true;
  this.emit('end');
}
```
- example usage
```shell
...
    }
  }
]
});

router.get(/foo/, function () {
this.res.writeHead(200, { 'Content-Type': 'text/plain' })
this.res.end('hello world\n');
});

router.post(/foo/, { stream: true }, function () {
var req = this.req,
    res = this.res,
    writeStream;
...
```

#### <a name="apidoc.element.union.BufferedStream.prototype.pause"></a>[function <span class="apidocSignatureSpan">union.BufferedStream.prototype.</span>pause ()](#apidoc.element.union.BufferedStream.prototype.pause)
- description and source-code
```javascript
pause = function () {
  this.emit('pause');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.BufferedStream.prototype.pipe"></a>[function <span class="apidocSignatureSpan">union.BufferedStream.prototype.</span>pipe ()](#apidoc.element.union.BufferedStream.prototype.pipe)
- description and source-code
```javascript
pipe = function () {
  var self = this,
      dest;

  if (self.resume) {
    self.resume();
  }

  dest = stream.Stream.prototype.pipe.apply(self, arguments);

  //
  // just incase you are piping to two streams, do not emit data twice.
  // note: you can pipe twice, but you need to pipe both streams in the same tick.
  // (this is normal for streams)
  //
  if (this.piped) {
    return dest;
  }

  process.nextTick(function () {
    if (self.chunks) {
      self.chunks.forEach(function (c) { self.emit('data', c) });
      self.size = 0;
      delete self.chunks;
    }

    if (!self.readable) {
      if (self.ended) {
        self.emit('end');
      }
      else if (self.closed) {
        self.emit('close');
      }
    }
  });

  this.piped = true;

  return dest;
}
```
- example usage
```shell
...

router.post(/foo/, { stream: true }, function () {
  var req = this.req,
      res = this.res,
      writeStream;

  writeStream = fs.createWriteStream(Date.now() + '-foo.txt');
  req.pipe(writeStream);

  writeStream.on('close', function () {
    res.writeHead(200, { 'Content-Type': 'text/plain' });
    res.end('wrote to a stream!');
  });
});
...
```

#### <a name="apidoc.element.union.BufferedStream.prototype.resume"></a>[function <span class="apidocSignatureSpan">union.BufferedStream.prototype.</span>resume ()](#apidoc.element.union.BufferedStream.prototype.resume)
- description and source-code
```javascript
resume = function () {
  this.emit('resume');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.BufferedStream.prototype.write"></a>[function <span class="apidocSignatureSpan">union.BufferedStream.prototype.</span>write (chunk)](#apidoc.element.union.BufferedStream.prototype.write)
- description and source-code
```javascript
write = function (chunk) {
  if (!this.chunks || this.piped) {
    this.emit('data', chunk);
    return;
  }

  this.chunks.push(chunk);
  this.size += chunk.length;
  if (this.limit < this.size) {
    this.pause();
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.union.HttpStream"></a>[module union.HttpStream](#apidoc.module.union.HttpStream)

#### <a name="apidoc.element.union.HttpStream.HttpStream"></a>[function <span class="apidocSignatureSpan">union.</span>HttpStream (options)](#apidoc.element.union.HttpStream.HttpStream)
- description and source-code
```javascript
HttpStream = function (options) {
  options = options || {};
  BufferedStream.call(this, options.limit);

  if (options.buffer === false) {
    this.buffer = false;
  }

  this.on('pipe', this.pipeState);
}
```
- example usage
```shell
...
'''
  function HttpStream()
'''

Example

'''js
var hs = union.HttpStream();
'''

## HttpStream Instance Members

### url
The url from the request.
...
```

#### <a name="apidoc.element.union.HttpStream.super_"></a>[function <span class="apidocSignatureSpan">union.HttpStream.</span>super_ (limit)](#apidoc.element.union.HttpStream.super_)
- description and source-code
```javascript
super_ = function (limit) {
  events.EventEmitter.call(this);

  if (typeof limit === 'undefined') {
    limit = Infinity;
  }

  this.limit = limit;
  this.size = 0;
  this.chunks = [];
  this.writable = true;
  this.readable = true;
  this._buffer = true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.union.HttpStream.prototype"></a>[module union.HttpStream.prototype](#apidoc.module.union.HttpStream.prototype)

#### <a name="apidoc.element.union.HttpStream.prototype.pipeState"></a>[function <span class="apidocSignatureSpan">union.HttpStream.prototype.</span>pipeState (source)](#apidoc.element.union.HttpStream.prototype.pipeState)
- description and source-code
```javascript
pipeState = function (source) {
  this.headers = source.headers;
  this.trailers = source.trailers;
  this.method = source.method;

  if (source.url) {
    this.url = this.originalUrl = source.url;
  }

  if (source.query) {
    this.query = source.query;
  }
  else if (source.url) {
    this.query = ~source.url.indexOf('?')
      ? qs.parse(url.parse(source.url).query)
      : {};
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.union.ResponseStream"></a>[module union.ResponseStream](#apidoc.module.union.ResponseStream)

#### <a name="apidoc.element.union.ResponseStream.ResponseStream"></a>[function <span class="apidocSignatureSpan">union.</span>ResponseStream (options)](#apidoc.element.union.ResponseStream.ResponseStream)
- description and source-code
```javascript
ResponseStream = function (options) {
  var self = this,
      key;

  options = options || {};
  HttpStream.call(this, options);

  this.writeable = true;
  this.response = options.response;

  if (options.headers) {
    for (key in options.headers) {
      this.response.setHeader(key, options.headers[key]);
    }
  }

  //
  // Proxy 'statusCode' changes to the actual 'response.statusCode'.
  //
  Object.defineProperty(this, 'statusCode', {
    get: function () {
      return self.response.statusCode;
    },
    set: function (value) {
      self.response.statusCode = value;
    },
    enumerable: true,
    configurable: true
  });

  if (this.response) {
    this._headers = this.response._headers = this.response._headers || {};

    // Patch to node core
    this.response._headerNames = this.response._headerNames || {};

    //
    // Proxy to emit "header" event
    //
    this._renderHeaders = this.response._renderHeaders;
    this.response._renderHeaders = function () {
      if (!self._emittedHeader) {
        self._emittedHeader = true;
        self.headerSent = true;
        self._header = true;
        self.emit('header');
      }

      return self._renderHeaders.call(self.response);
    };
  }
}
```
- example usage
```shell
...
'''
  function ResponseStream()
'''

Example

'''js
var rs = union.ResponseStream();
'''

# Tests

All tests are written with [vows][0] and should be run with [npm][1]:

''' bash
...
```

#### <a name="apidoc.element.union.ResponseStream.super_"></a>[function <span class="apidocSignatureSpan">union.ResponseStream.</span>super_ (options)](#apidoc.element.union.ResponseStream.super_)
- description and source-code
```javascript
super_ = function (options) {
  options = options || {};
  BufferedStream.call(this, options.limit);

  if (options.buffer === false) {
    this.buffer = false;
  }

  this.on('pipe', this.pipeState);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.union.ResponseStream.prototype"></a>[module union.ResponseStream.prototype](#apidoc.module.union.ResponseStream.prototype)

#### <a name="apidoc.element.union.ResponseStream.prototype._implicitHeader"></a>[function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>_implicitHeader ()](#apidoc.element.union.ResponseStream.prototype._implicitHeader)
- description and source-code
```javascript
_implicitHeader = function () {
  return this.response[method].apply(this.response, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.ResponseStream.prototype.addTrailers"></a>[function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>addTrailers ()](#apidoc.element.union.ResponseStream.prototype.addTrailers)
- description and source-code
```javascript
addTrailers = function () {
  return this.response[method].apply(this.response, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.ResponseStream.prototype.end"></a>[function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>end (data)](#apidoc.element.union.ResponseStream.prototype.end)
- description and source-code
```javascript
end = function (data) {
  if (data && this.writable) {
    this.emit('data', data);
  }

  this.modified = true;
  this.emit('end');
}
```
- example usage
```shell
...
    }
  }
]
});

router.get(/foo/, function () {
this.res.writeHead(200, { 'Content-Type': 'text/plain' })
this.res.end('hello world\n');
});

router.post(/foo/, { stream: true }, function () {
var req = this.req,
    res = this.res,
    writeStream;
...
```

#### <a name="apidoc.element.union.ResponseStream.prototype.getHeader"></a>[function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>getHeader ()](#apidoc.element.union.ResponseStream.prototype.getHeader)
- description and source-code
```javascript
getHeader = function () {
  return this.response[method].apply(this.response, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.ResponseStream.prototype.html"></a>[function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>html (str)](#apidoc.element.union.ResponseStream.prototype.html)
- description and source-code
```javascript
html = function (str) {
  if (!this.response.writable) {
    return;
  }

  if (typeof str === 'number') {
    this.response.statusCode = str;
    str = arguments[1];
  }

  this.modified = true;

  if (!this.response._header && this.response.getHeader('content-type') !== 'text/html') {
    this.response.setHeader('content-type', 'text/html');
  }

  this.end(str ? str: '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.ResponseStream.prototype.json"></a>[function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>json (obj)](#apidoc.element.union.ResponseStream.prototype.json)
- description and source-code
```javascript
json = function (obj) {
  if (!this.response.writable) {
    return;
  }

  if (typeof obj === 'number') {
    this.response.statusCode = obj;
    obj = arguments[1];
  }

  this.modified = true;

  if (!this.response._header && this.response.getHeader('content-type') !== 'application/json') {
    this.response.setHeader('content-type', 'application/json');
  }

  this.end(obj ? JSON.stringify(obj) : '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.ResponseStream.prototype.pipe"></a>[function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>pipe ()](#apidoc.element.union.ResponseStream.prototype.pipe)
- description and source-code
```javascript
pipe = function () {
  var self = this,
      dest;

  self.dest = dest = HttpStream.prototype.pipe.apply(self, arguments);

  dest.on('drain', function() {
    self.emit('drain')
  })
  return dest;
}
```
- example usage
```shell
...

router.post(/foo/, { stream: true }, function () {
  var req = this.req,
      res = this.res,
      writeStream;

  writeStream = fs.createWriteStream(Date.now() + '-foo.txt');
  req.pipe(writeStream);

  writeStream.on('close', function () {
    res.writeHead(200, { 'Content-Type': 'text/plain' });
    res.end('wrote to a stream!');
  });
});
...
```

#### <a name="apidoc.element.union.ResponseStream.prototype.redirect"></a>[function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>redirect (path, status)](#apidoc.element.union.ResponseStream.prototype.redirect)
- description and source-code
```javascript
redirect = function (path, status) {
  var url = '';

  if (~path.indexOf('://')) {
    url = path;
  } else {
    url += this.req.connection.encrypted ? 'https://' : 'http://';
    url += this.req.headers.host;
    url += (path[0] === '/') ? path : '/' + path;
  }

  this.res.writeHead(status || 302, { 'Location': url });
  this.end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.ResponseStream.prototype.removeHeader"></a>[function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>removeHeader ()](#apidoc.element.union.ResponseStream.prototype.removeHeader)
- description and source-code
```javascript
removeHeader = function () {
  return this.response[method].apply(this.response, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.ResponseStream.prototype.setHeader"></a>[function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>setHeader ()](#apidoc.element.union.ResponseStream.prototype.setHeader)
- description and source-code
```javascript
setHeader = function () {
  return this.response[method].apply(this.response, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.ResponseStream.prototype.text"></a>[function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>text (str)](#apidoc.element.union.ResponseStream.prototype.text)
- description and source-code
```javascript
text = function (str) {
  if (!this.response.writable) {
    return;
  }

  if (typeof str === 'number') {
    this.response.statusCode = str;
    str = arguments[1];
  }

  this.modified = true;

  if (!this.response._header && this.response.getHeader('content-type') !== 'text/plain') {
    this.response.setHeader('content-type', 'text/plain');
  }

  this.end(str ? str: '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.ResponseStream.prototype.write"></a>[function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>write (data)](#apidoc.element.union.ResponseStream.prototype.write)
- description and source-code
```javascript
write = function (data) {
  this.modified = true;

  if (this.writable) {
    return this.dest.write(data);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.ResponseStream.prototype.writeHead"></a>[function <span class="apidocSignatureSpan">union.ResponseStream.prototype.</span>writeHead (statusCode, statusMessage, headers)](#apidoc.element.union.ResponseStream.prototype.writeHead)
- description and source-code
```javascript
writeHead = function (statusCode, statusMessage, headers) {
  if (typeof statusMessage === 'string') {
    this.response.statusMessage = statusMessage;
  } else {
    this.response.statusMessage = this.response.statusMessage
      || STATUS_CODES[statusCode] || 'unknown';
    headers = statusMessage;
  }

  this.response.statusCode = statusCode;

  if (headers) {
    var keys = Object.keys(headers);
    for (var i = 0; i < keys.length; i++) {
      var k = keys[i];
      if (k) this.response.setHeader(k, headers[k]);
    }
  }
}
```
- example usage
```shell
...
      res.emit('next');
    }
  }
]
});

router.get(/foo/, function () {
this.res.writeHead(200, { 'Content-Type': 'text/plain' })
this.res.end('hello world\n');
});

router.post(/foo/, { stream: true }, function () {
var req = this.req,
    res = this.res,
    writeStream;
...
```



# <a name="apidoc.module.union.RoutingStream"></a>[module union.RoutingStream](#apidoc.module.union.RoutingStream)

#### <a name="apidoc.element.union.RoutingStream.RoutingStream"></a>[function <span class="apidocSignatureSpan">union.</span>RoutingStream (options)](#apidoc.element.union.RoutingStream.RoutingStream)
- description and source-code
```javascript
RoutingStream = function (options) {
  options = options || {};
  RequestStream.call(this, options);

  this.before = options.before || [];
  this.after = options.after || [];
  this.response = options.response || options.res;
  this.headers = options.headers || {
    'x-powered-by': 'union ' + union.version
  };

  this.target = new ResponseStream({
    response: this.response,
    headers: this.headers
  });

  this.once('pipe', this.route);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.RoutingStream.super_"></a>[function <span class="apidocSignatureSpan">union.RoutingStream.</span>super_ (options)](#apidoc.element.union.RoutingStream.super_)
- description and source-code
```javascript
super_ = function (options) {
  options = options || {};
  HttpStream.call(this, options);

  this.on('pipe', this.pipeRequest);
  this.request = options.request;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.union.RoutingStream.prototype"></a>[module union.RoutingStream.prototype](#apidoc.module.union.RoutingStream.prototype)

#### <a name="apidoc.element.union.RoutingStream.prototype.onError"></a>[function <span class="apidocSignatureSpan">union.RoutingStream.prototype.</span>onError (err)](#apidoc.element.union.RoutingStream.prototype.onError)
- description and source-code
```javascript
onError = function (err) {
  this.emit('error', err);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.RoutingStream.prototype.route"></a>[function <span class="apidocSignatureSpan">union.RoutingStream.prototype.</span>route (req)](#apidoc.element.union.RoutingStream.prototype.route)
- description and source-code
```javascript
route = function (req) {
  //
  // When a 'RoutingStream' is piped to:
  //
  // 1. Setup the pipe-chain between the 'after' middleware, the abstract response
  //    and the concrete response.
  // 2. Attempt to dispatch to the 'before' middleware, which represent things such as
  //    favicon, static files, application routing.
  // 3. If no match is found then pipe to the 404Stream
  //
  var self = this,
      after,
      error,
      i;

  //
  // Don't allow 'this.target' to be writable on HEAD requests
  //
  this.target.writable = req.method !== 'HEAD';

  //
  // 1. Setup the pipe-chain between the 'after' middleware, the abstract response
  //    and the concrete response.
  //
  after = [this.target].concat(this.after, this.response);
  for (i = 0; i < after.length - 1; i++) {
    //
    // attach req and res to all streams
    //
    after[i].req     = req;
    after[i + 1].req = req;
    after[i].res     = this.response;
    after[i + 1].res = this.response;
    after[i].pipe(after[i + 1]);

    //
    // prevent multiple responses and memory leaks
    //
    after[i].on('error', this.onError);
  }

  //
  // Helper function for dispatching to the 404 stream.
  //
  function notFound() {
    error = new Error('Not found');
    error.status = 404;
    self.onError(error);
  }

  //
  // 2. Attempt to dispatch to the 'before' middleware, which represent things such as
  //    favicon, static files, application routing.
  //
  (function dispatch(i) {
    if (self.target.modified) {
      return;
    }
    else if (++i === self.before.length) {
      //
      // 3. If no match is found then pipe to the 404Stream
      //
      return notFound();
    }

    self.target.once('next', dispatch.bind(null, i));
    if (self.before[i].length === 3) {
      self.before[i](self, self.target, function (err) {
        if (err) {
          self.onError(err);
        } else {
          self.target.emit('next');
        }
      });
    }
    else {
      self.before[i](self, self.target);
    }
  })(-1);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.union.RoutingStream.super_"></a>[module union.RoutingStream.super_](#apidoc.module.union.RoutingStream.super_)

#### <a name="apidoc.element.union.RoutingStream.super_.super_"></a>[function <span class="apidocSignatureSpan">union.RoutingStream.</span>super_ (options)](#apidoc.element.union.RoutingStream.super_.super_)
- description and source-code
```javascript
super_ = function (options) {
  options = options || {};
  BufferedStream.call(this, options.limit);

  if (options.buffer === false) {
    this.buffer = false;
  }

  this.on('pipe', this.pipeState);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.union.RoutingStream.super_.prototype"></a>[module union.RoutingStream.super_.prototype](#apidoc.module.union.RoutingStream.super_.prototype)

#### <a name="apidoc.element.union.RoutingStream.super_.prototype.pipeRequest"></a>[function <span class="apidocSignatureSpan">union.RoutingStream.super_.prototype.</span>pipeRequest (source)](#apidoc.element.union.RoutingStream.super_.prototype.pipeRequest)
- description and source-code
```javascript
pipeRequest = function (source) {
  this.url = this.originalUrl = source.url;
  this.method = source.method;
  this.httpVersion = source.httpVersion;
  this.httpVersionMajor = source.httpVersionMajor;
  this.httpVersionMinor = source.httpVersionMinor;
  this.setEncoding = source.setEncoding;
  this.connection = source.connection;
  this.socket = source.socket;

  if (source.query) {
    this.query = source.query;
  }
  else {
    this.query = ~source.url.indexOf('?')
      ? qs.parse(url.parse(source.url).query)
      : {};
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.union.RoutingStream.super_.prototype.setEncoding"></a>[function <span class="apidocSignatureSpan">union.RoutingStream.super_.prototype.</span>setEncoding ()](#apidoc.element.union.RoutingStream.super_.prototype.setEncoding)
- description and source-code
```javascript
setEncoding = function () {
  return this.request[method].apply(this.request, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.union.core"></a>[module union.core](#apidoc.module.union.core)

#### <a name="apidoc.element.union.core.createServer"></a>[function <span class="apidocSignatureSpan">union.core.</span>createServer (options)](#apidoc.element.union.core.createServer)
- description and source-code
```javascript
createServer = function (options) {
  var isArray = Array.isArray(options.after),
      credentials;

  if (!options) {
    throw new Error('options is required to create a server');
  }

  function requestHandler(req, res) {
    var routingStream = new RoutingStream({
      before: options.before,
      buffer: options.buffer,
      //
      // Remark: without new after is a huge memory leak that
      // pipes to every single open connection
      //
      after: isArray && options.after.map(function (After) {
        return new After;
      }),
      request: req,
      response: res,
      limit: options.limit,
      headers: options.headers
    });

    routingStream.on('error', function (err) {
      var fn = options.onError || core.errorHandler;
      fn(err, routingStream, routingStream.target, function () {
        routingStream.target.emit('next');
      });
    });

    req.pipe(routingStream);
  }

  //
  // both https and spdy requires same params
  //
  if (options.https || options.spdy) {
    if (options.https && options.spdy) {
      throw new Error('You shouldn\'t be using https and spdy simultaneously.');
    }

    var serverOptions,
        credentials,
        key = !options.spdy
          ? 'https'
          : 'spdy';

    serverOptions = options[key];
    if (!serverOptions.key || !serverOptions.cert) {
      throw new Error('Both options.' + key + '.'key' and options.' + key + '.'cert' are required.');
    }

    credentials = {
      key:  fs.readFileSync(serverOptions.key),
      cert: fs.readFileSync(serverOptions.cert)
    };

    if (serverOptions.ca) {
      serverOptions.ca = !Array.isArray(serverOptions.ca)
        ? [serverOptions.ca]
        : serverOptions.ca

      credentials.ca = serverOptions.ca.map(function (ca) {
        return fs.readFileSync(ca);
      });
    }

    if (options.spdy) {
      // spdy is optional so we require module here rather than on top
      var spdy = require('spdy');
      return spdy.createServer(credentials, requestHandler);
    }

    return https.createServer(credentials, requestHandler);
  }

  return http.createServer(requestHandler);
}
```
- example usage
```shell
...
''' js
var fs = require('fs'),
  union = require('../lib'),
  director = require('director');

var router = new director.http.Router();

var server = union.createServer({
before: [
  function (req, res) {
    var found = router.dispatch(req, res);
    if (!found) {
      res.emit('next');
    }
  }
...
```

#### <a name="apidoc.element.union.core.errorHandler"></a>[function <span class="apidocSignatureSpan">union.core.</span>errorHandler (err, req, res)](#apidoc.element.union.core.errorHandler)
- description and source-code
```javascript
function error(err, req, res) {
  if (err) {
    (this.res || res).writeHead(err.status || 500, err.headers || { "Content-Type": "text/plain" });
    (this.res || res).end(err.message + "\n");
    return;
  }

  (this.res || res).writeHead(404, {"Content-Type": "text/plain"});
  (this.res || res).end("Not Found\n");
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
