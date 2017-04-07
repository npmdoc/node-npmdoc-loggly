# api documentation for  [loggly (v1.1.1)](https://github.com/winstonjs/node-loggly#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-loggly.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-loggly) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-loggly.svg)](https://travis-ci.org/npmdoc/node-npmdoc-loggly)
#### A client implementation for Loggly cloud Logging-as-a-Service API

[![NPM](https://nodei.co/npm/loggly.png?downloads=true)](https://www.npmjs.com/package/loggly)

[![apidoc](https://npmdoc.github.io/node-npmdoc-loggly/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-loggly_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-loggly/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-loggly/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-loggly/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Charlie Robbins",
        "email": "charlie.robbins@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/winstonjs/node-loggly/issues"
    },
    "dependencies": {
        "json-stringify-safe": "5.0.x",
        "request": "2.75.x",
        "timespan": "2.3.x"
    },
    "description": "A client implementation for Loggly cloud Logging-as-a-Service API",
    "devDependencies": {
        "common-style": "^3.1.0",
        "vows": "0.8.x"
    },
    "directories": {},
    "dist": {
        "shasum": "0a0fc1d3fa3a5ec44fdc7b897beba2a4695cebee",
        "tarball": "https://registry.npmjs.org/loggly/-/loggly-1.1.1.tgz"
    },
    "engines": {
        "node": ">= 0.8.0"
    },
    "gitHead": "34c562bcb584b42cab4298c30151707ab5788137",
    "homepage": "https://github.com/winstonjs/node-loggly#readme",
    "keywords": [
        "cloud computing",
        "api",
        "logging",
        "loggly"
    ],
    "license": "MIT",
    "main": "./lib/loggly",
    "maintainers": [
        {
            "name": "indexzero",
            "email": "charlie.robbins@gmail.com"
        },
        {
            "name": "jcrugzz",
            "email": "jcrugzz@gmail.com"
        }
    ],
    "name": "loggly",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/winstonjs/node-loggly.git"
    },
    "scripts": {
        "pretest": "common lib/**/*.js lib/*.js test/helpers.js",
        "test": "vows test/*-test.js --spec"
    },
    "version": "1.1.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module loggly](#apidoc.module.loggly)
1.  [function <span class="apidocSignatureSpan">loggly.</span>Loggly (options)](#apidoc.element.loggly.Loggly)
1.  [function <span class="apidocSignatureSpan">loggly.</span>Search (options, client)](#apidoc.element.loggly.Search)
1.  [function <span class="apidocSignatureSpan">loggly.</span>createClient (options)](#apidoc.element.loggly.createClient)
1.  [function <span class="apidocSignatureSpan">loggly.</span>serialize (obj, key)](#apidoc.element.loggly.serialize)
1.  object <span class="apidocSignatureSpan">loggly.</span>Loggly.prototype
1.  object <span class="apidocSignatureSpan">loggly.</span>Search.prototype
1.  string <span class="apidocSignatureSpan">loggly.</span>version

#### [module loggly.Loggly](#apidoc.module.loggly.Loggly)
1.  [function <span class="apidocSignatureSpan">loggly.</span>Loggly (options)](#apidoc.element.loggly.Loggly.Loggly)
1.  [function <span class="apidocSignatureSpan">loggly.Loggly.</span>super_ ()](#apidoc.element.loggly.Loggly.super_)

#### [module loggly.Loggly.prototype](#apidoc.module.loggly.Loggly.prototype)
1.  [function <span class="apidocSignatureSpan">loggly.Loggly.prototype.</span>customer (callback)](#apidoc.element.loggly.Loggly.prototype.customer)
1.  [function <span class="apidocSignatureSpan">loggly.Loggly.prototype.</span>log (msg, tags, callback)](#apidoc.element.loggly.Loggly.prototype.log)
1.  [function <span class="apidocSignatureSpan">loggly.Loggly.prototype.</span>logglyUrl ()](#apidoc.element.loggly.Loggly.prototype.logglyUrl)
1.  [function <span class="apidocSignatureSpan">loggly.Loggly.prototype.</span>search (query, callback)](#apidoc.element.loggly.Loggly.prototype.search)
1.  [function <span class="apidocSignatureSpan">loggly.Loggly.prototype.</span>tagFilter (tags)](#apidoc.element.loggly.Loggly.prototype.tagFilter)

#### [module loggly.Search](#apidoc.module.loggly.Search)
1.  [function <span class="apidocSignatureSpan">loggly.</span>Search (options, client)](#apidoc.element.loggly.Search.Search)
1.  [function <span class="apidocSignatureSpan">loggly.Search.</span>super_ ()](#apidoc.element.loggly.Search.super_)

#### [module loggly.Search.prototype](#apidoc.module.loggly.Search.prototype)
1.  [function <span class="apidocSignatureSpan">loggly.Search.prototype.</span>_checkRange ()](#apidoc.element.loggly.Search.prototype._checkRange)
1.  [function <span class="apidocSignatureSpan">loggly.Search.prototype.</span>run (callback)](#apidoc.element.loggly.Search.prototype.run)



# <a name="apidoc.module.loggly"></a>[module loggly](#apidoc.module.loggly)

#### <a name="apidoc.element.loggly.Loggly"></a>[function <span class="apidocSignatureSpan">loggly.</span>Loggly (options)](#apidoc.element.loggly.Loggly)
- description and source-code
```javascript
Loggly = function (options) {
  if (!options || !options.subdomain || !options.token) {
    throw new Error('options.subdomain and options.token are required.');
  }

  events.EventEmitter.call(this);
  this.subdomain    = options.subdomain;
  this.token        = options.token;
  this.host         = options.host || 'logs-01.loggly.com';
  this.json         = options.json || null;
  this.auth         = options.auth || null;
  this.proxy        = options.proxy || null;
  this.userAgent    = 'node-loggly ' + loggly.version;
  this.useTagHeader = 'useTagHeader' in options ? options.useTagHeader : true;

  //
  // Set the tags on this instance.
  //
  this.tags = options.tags
    ? this.tagFilter(options.tags)
    : null;

  var url   = 'https://' + this.host,
      api   = options.api  || 'apiv2';

  this.urls = {
    default: url,
    log:     [url, 'inputs', this.token].join('/'),
    bulk:    [url, 'bulk', this.token].join('/'),
    api:     'https://' + [this.subdomain, 'loggly', 'com'].join('.') + '/' + api
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.loggly.Search"></a>[function <span class="apidocSignatureSpan">loggly.</span>Search (options, client)](#apidoc.element.loggly.Search)
- description and source-code
```javascript
Search = function (options, client) {
  if (!options || (!options.query && !options.q)) {
    throw new Error('options.query is required to execute a Loggly search.');
  }

  events.EventEmitter.call(this);

  if (options.query) {
    options.q = options.query;
    delete options.query;
  }

  this.options = options;
  this.client  = client;

  //
  // If we're passed a callback, run immediately.
  //
  if (options.callback) {
    this.callback = options.callback;
    delete options.callback;
    this.run();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.loggly.createClient"></a>[function <span class="apidocSignatureSpan">loggly.</span>createClient (options)](#apidoc.element.loggly.createClient)
- description and source-code
```javascript
createClient = function (options) {
  return new Loggly(options);
}
```
- example usage
```shell
...

### Getting Started
Before we can do anything with Loggly, we have to create a client with valid credentials. We will authenticate for you automatically
:

''' js
var loggly = require('loggly');

var client = loggly.createClient({
  token: "your-really-long-input-token",
  subdomain: "your-subdomain",
  auth: {
    username: "your-username",
    password: "your-password"
  },
  //
...
```

#### <a name="apidoc.element.loggly.serialize"></a>[function <span class="apidocSignatureSpan">loggly.</span>serialize (obj, key)](#apidoc.element.loggly.serialize)
- description and source-code
```javascript
serialize = function (obj, key) {
  if (obj === null) {
    obj = 'null';
  }
  else if (obj === undefined) {
    obj = 'undefined';
  }
  else if (obj === false) {
    obj = 'false';
  }

  if (typeof obj !== 'object') {
    return key ? key + '=' + obj : obj;
  }

  var msg = '',
      keys = Object.keys(obj),
      length = keys.length;

  for (var i = 0; i < length; i++) {
    if (Array.isArray(obj[keys[i]])) {
      msg += keys[i] + '=[';

      for (var j = 0, l = obj[keys[i]].length; j < l; j++) {
        msg += common.serialize(obj[keys[i]][j]);
        if (j < l - 1) {
          msg += ', ';
        }
      }

      msg += ']';
    }
    else {
      msg += common.serialize(obj[keys[i]], keys[i]);
    }

    if (i < length - 1) {
      msg += ', ';
    }
  }

  return msg;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.loggly.Loggly"></a>[module loggly.Loggly](#apidoc.module.loggly.Loggly)

#### <a name="apidoc.element.loggly.Loggly.Loggly"></a>[function <span class="apidocSignatureSpan">loggly.</span>Loggly (options)](#apidoc.element.loggly.Loggly.Loggly)
- description and source-code
```javascript
Loggly = function (options) {
  if (!options || !options.subdomain || !options.token) {
    throw new Error('options.subdomain and options.token are required.');
  }

  events.EventEmitter.call(this);
  this.subdomain    = options.subdomain;
  this.token        = options.token;
  this.host         = options.host || 'logs-01.loggly.com';
  this.json         = options.json || null;
  this.auth         = options.auth || null;
  this.proxy        = options.proxy || null;
  this.userAgent    = 'node-loggly ' + loggly.version;
  this.useTagHeader = 'useTagHeader' in options ? options.useTagHeader : true;

  //
  // Set the tags on this instance.
  //
  this.tags = options.tags
    ? this.tagFilter(options.tags)
    : null;

  var url   = 'https://' + this.host,
      api   = options.api  || 'apiv2';

  this.urls = {
    default: url,
    log:     [url, 'inputs', this.token].join('/'),
    bulk:    [url, 'bulk', this.token].join('/'),
    api:     'https://' + [this.subdomain, 'loggly', 'com'].join('.') + '/' + api
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.loggly.Loggly.super_"></a>[function <span class="apidocSignatureSpan">loggly.Loggly.</span>super_ ()](#apidoc.element.loggly.Loggly.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.loggly.Loggly.prototype"></a>[module loggly.Loggly.prototype](#apidoc.module.loggly.Loggly.prototype)

#### <a name="apidoc.element.loggly.Loggly.prototype.customer"></a>[function <span class="apidocSignatureSpan">loggly.Loggly.prototype.</span>customer (callback)](#apidoc.element.loggly.Loggly.prototype.customer)
- description and source-code
```javascript
customer = function (callback) {
  common.loggly({
    uri: this.logglyUrl('customer'),
    auth: this.auth
  }, callback, function (res, body) {
    var customer;
    try { customer = JSON.parse(body) }
    catch (ex) { return callback(ex) }
    callback(null, customer);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.loggly.Loggly.prototype.log"></a>[function <span class="apidocSignatureSpan">loggly.Loggly.prototype.</span>log (msg, tags, callback)](#apidoc.element.loggly.Loggly.prototype.log)
- description and source-code
```javascript
log = function (msg, tags, callback) {
  if (!callback && typeof tags === 'function') {
    callback = tags;
    tags = null;
  }

  var self = this,
      logOptions;

  //
  // Remark: Have some extra logic for detecting if we want to make a bulk
  // request to loggly
  //
  var isBulk = Array.isArray(msg);
  function serialize(msg) {
    if (msg instanceof Object) {
      return self.json ? stringify(msg) : common.serialize(msg);
    }
    else {
      return self.json ? stringify({ message: msg }) : msg;
    }
  }

  msg = isBulk ? msg.map(serialize).join('\n') : serialize(msg);

  logOptions = {
    uri:     isBulk ? this.urls.bulk : this.urls.log,
    method:  'POST',
    body:    msg,
    proxy:   this.proxy,
    headers: {
      host:             this.host,
      accept:           '*/*',
      'user-agent':     this.userAgent,
      'content-type':   this.json ? 'application/json' : 'text/plain',
      'content-length': Buffer.byteLength(msg)
    }
  };

  //
  // Remark: if tags are passed in run the filter on them and concat
  // with any tags that were passed or just use default tags if they exist
  //
  tags = tags
    ? (this.tags ? this.tags.concat(this.tagFilter(tags)) : this.tagFilter(tags))
    : this.tags;

  //
  // Optionally send 'X-LOGGLY-TAG' if we have them
  //
  if (tags) {
    // Decide whether to add tags as http headers or add them to the URI.
    if (this.useTagHeader) {
      logOptions.headers['X-LOGGLY-TAG'] = tags.join(',');
    }
    else {
      logOptions.uri += '/tag/' + tags.join(',') + '/';
    }
  }

  common.loggly(logOptions, callback, function (res, body) {
    try {
      var result = JSON.parse(body);
      self.emit('log', result);
      if (callback) {
        callback(null, result);
      }
    }
    catch (ex) {
      if (callback) {
        callback(new Error('Unspecified error from Loggly: ' + ex));
      }
    }
  });

  return this;
}
```
- example usage
```shell
...
  });
'''

### Logging
There are two ways to send log information to Loggly via node-loggly. The first is to simply call client.log with an appropriate
 input token:

''' js
  client.log('127.0.0.1 - Theres no place like home', function (err, result) {
    // Do something once you've logged
  });
'''

Note that the callback in the above example is optional, if you prefer the 'fire and forget' method of logging:

''' js
...
```

#### <a name="apidoc.element.loggly.Loggly.prototype.logglyUrl"></a>[function <span class="apidocSignatureSpan">loggly.Loggly.prototype.</span>logglyUrl ()](#apidoc.element.loggly.Loggly.prototype.logglyUrl)
- description and source-code
```javascript
logglyUrl = function () {
  var args = Array.prototype.slice.call(arguments);
  return [this.urls.api].concat(args).join('/');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.loggly.Loggly.prototype.search"></a>[function <span class="apidocSignatureSpan">loggly.Loggly.prototype.</span>search (query, callback)](#apidoc.element.loggly.Loggly.prototype.search)
- description and source-code
```javascript
search = function (query, callback) {
  var options = typeof query === 'string'
    ? { query: query }
    : query;

  options.callback = callback;
  return new Search(options, this);
}
```
- example usage
```shell
...

### Searching
[Searching][search-api] with node-loggly is easy. All you have to do is use the search() method defined on each Loggly client:

''' js
  var util = require('util');

  client.search('404', function (err, results) {
    // Inspect the result set
    console.dir(results.events);
  });
'''

The search() method can also take an Object parameter that allows you to set additional search parameters such as: rows, from, until
, etc.
...
```

#### <a name="apidoc.element.loggly.Loggly.prototype.tagFilter"></a>[function <span class="apidocSignatureSpan">loggly.Loggly.prototype.</span>tagFilter (tags)](#apidoc.element.loggly.Loggly.prototype.tagFilter)
- description and source-code
```javascript
tagFilter = function (tags) {
  var isSolid = /^[\w\d][\w\d-_.]+/;

  tags = !Array.isArray(tags)
    ? [tags]
    : tags;

  //
  // TODO: Filter against valid tag names with some Regex
  // http://www.loggly.com/docs/tags/
  // Remark: Docs make me think we dont need this but whatevs
  //
  return tags.filter(function (tag) {
    //
    // Remark: length may need to use Buffer.byteLength?
    //
    return isSolid.test(tag) && tag.length <= 64;
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.loggly.Search"></a>[module loggly.Search](#apidoc.module.loggly.Search)

#### <a name="apidoc.element.loggly.Search.Search"></a>[function <span class="apidocSignatureSpan">loggly.</span>Search (options, client)](#apidoc.element.loggly.Search.Search)
- description and source-code
```javascript
Search = function (options, client) {
  if (!options || (!options.query && !options.q)) {
    throw new Error('options.query is required to execute a Loggly search.');
  }

  events.EventEmitter.call(this);

  if (options.query) {
    options.q = options.query;
    delete options.query;
  }

  this.options = options;
  this.client  = client;

  //
  // If we're passed a callback, run immediately.
  //
  if (options.callback) {
    this.callback = options.callback;
    delete options.callback;
    this.run();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.loggly.Search.super_"></a>[function <span class="apidocSignatureSpan">loggly.Search.</span>super_ ()](#apidoc.element.loggly.Search.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.loggly.Search.prototype"></a>[module loggly.Search.prototype](#apidoc.module.loggly.Search.prototype)

#### <a name="apidoc.element.loggly.Search.prototype._checkRange"></a>[function <span class="apidocSignatureSpan">loggly.Search.prototype.</span>_checkRange ()](#apidoc.element.loggly.Search.prototype._checkRange)
- description and source-code
```javascript
_checkRange = function () {
  if (!this.options.until && !this.options.from) {
    return;
  }

  this.options.until = this.options.until || 'now';
  this.options.from  = this.options.from  || '-24h';

  if (!timespan.parseDate(this.options.until)) {
    this.options.until = 'now';
  }

  if (!timespan.parseDate(this.options.from)) {
    this.options.from = '-24h';
  }

  if (timespan.fromDates(this.options.from, this.options.until) < 0
    || this.options.until === this.options.from) {
    //
    // If the length of the timespan for this Search instance is
    // negative then set it to default values
    //
    this.options.until = 'now';
    this.options.from = '-24h';
  }

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.loggly.Search.prototype.run"></a>[function <span class="apidocSignatureSpan">loggly.Search.prototype.</span>run (callback)](#apidoc.element.loggly.Search.prototype.run)
- description and source-code
```javascript
run = function (callback) {
  var self = this,
      responded;

  //
  // Trim the search query
  //
  this.options.q.trim();

  //
  // Update the callback for this instance if it's passed
  //
  this.callback = callback || this.callback;
  if (!this.callback) {
    throw new Error('Cannot run search without a callback function.');
  }

  //
  // ### function respond (arguments...)
  // Responds only once.
  //
  function respond() {
    if (!responded) {
      responded = true;
      self.callback.apply(null, arguments);
    }
  }

  //
  // ### function awaitResults (rsid)
  // Checks the Loggly API on an interval for the
  // results from the specified 'rsid'.
  //
  function awaitResults(rsid) {
    if (!rsid || !rsid.id) {
      return respond(rsid);
    }

    common.loggly({
      uri:  self.client.logglyUrl('events?' + qs.stringify({ rsid: rsid.id })),
      auth: self.client.auth,
      json: true
    }, respond, function (res, body) {
      var results;
      try { results = JSON.parse(body) }
      catch (ex) { return respond(ex) }
      respond(null, results);
    });
  }

  //
  // Check any time ranges (if supplied) to ensure
  // they are valid.
  //
  this._checkRange();

  common.loggly({
    uri:  this.client.logglyUrl('search?' + qs.stringify(this.options)),
    auth: this.client.auth,
    json: true
  }, this.callback, function (res, body) {
    var rsid;
    try { rsid = JSON.parse(body).rsid }
    catch (ex) { rsid = ex }

    self.emit('rsid', rsid);
    awaitResults(rsid);
  });

  return this;
}
```
- example usage
```shell
...

The search() method can also take an Object parameter that allows you to set additional search parameters such as: rows, from, until
, etc.

''' js
  var util = require('util');

  client.search({ query: '404', rows: 10 })
    .run(function (err, results) {
      // Inspect the result set
      console.dir(results.events);
    });
'''

See the [Loggly search guide][search] for more details on how to effectively search through your Loggly logs.
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
