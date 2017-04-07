# api documentation for  [thepiratebay (v1.3.5)](http://github.com/t3chnoboy/thepiratebay)  [![npm package](https://img.shields.io/npm/v/npmdoc-thepiratebay.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-thepiratebay) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-thepiratebay.svg)](https://travis-ci.org/npmdoc/node-npmdoc-thepiratebay)
#### The pirate bay client

[![NPM](https://nodei.co/npm/thepiratebay.png?downloads=true)](https://www.npmjs.com/package/thepiratebay)

[![apidoc](https://npmdoc.github.io/node-npmdoc-thepiratebay/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-thepiratebay_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-thepiratebay/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-thepiratebay/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-thepiratebay/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Dmitry Mazuro",
        "email": "dmitry.mazuro@icloud.com"
    },
    "bugs": {
        "url": "https://github.com/t3chnoboy/thepiratebay/issues"
    },
    "dependencies": {
        "babel-runtime": "^6.23.0",
        "cheerio": "^0.22.0",
        "isomorphic-fetch": "^2.2.1",
        "url-parse": "^1.1.8"
    },
    "description": "The pirate bay client",
    "devDependencies": {
        "babel-cli": "^6.24.0",
        "babel-eslint": "^7.2.1",
        "babel-loader": "^6.4.1",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-transform-es2015-modules-umd": "^6.24.0",
        "babel-plugin-transform-flow-strip-types": "^6.22.0",
        "babel-plugin-transform-runtime": "^6.23.0",
        "babel-polyfill": "^6.23.0",
        "babel-preset-es2015": "^6.24.0",
        "babel-preset-latest": "^6.24.0",
        "babel-preset-stage-0": "^6.22.0",
        "babel-register": "^6.24.0",
        "chai": "^3.5.0",
        "cross-env": "^3.2.4",
        "eslint": "^3.18.0",
        "eslint-config-bliss": "^1.0.3",
        "eslint-formatter-pretty": "^1.1.0",
        "flow-bin": "^0.42.0",
        "flow-typed": "^2.0.0",
        "jest-cli": "^19.0.2",
        "json-loader": "^0.5.4"
    },
    "devEngines": {
        "node": ">=4.x",
        "npm": ">=3.x"
    },
    "directories": {},
    "dist": {
        "shasum": "818acb57f178d989c928c2e3498ef7223cad86a3",
        "tarball": "https://registry.npmjs.org/thepiratebay/-/thepiratebay-1.3.5.tgz"
    },
    "engines": {
        "node": ">=4.x",
        "npm": ">=3.x"
    },
    "files": [
        "lib"
    ],
    "gitHead": "238e655363c1d8949442bc4a2822c80eb11d377c",
    "homepage": "http://github.com/t3chnoboy/thepiratebay",
    "jest": {
        "testEnvironment": "node"
    },
    "keywords": [
        "thepiratebay",
        "pirate bay",
        "torrent",
        "api",
        "client",
        "scraper"
    ],
    "license": "MIT",
    "main": "./lib/PirateBay.js",
    "maintainers": [
        {
            "name": "t3chnoboy",
            "email": "dmitry.mazuro@icloud.com"
        },
        {
            "name": "redbackthomson",
            "email": "redback93@hotmail.com"
        }
    ],
    "name": "thepiratebay",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/t3chnoboy/thepiratebay.git"
    },
    "scripts": {
        "build": "cross-env NODE_ENV=production babel src --out-dir lib",
        "clean": "rm -rf lib",
        "flow": "flow check",
        "flow-typed": "flow-typed install",
        "lint": "eslint --cache --format=node_modules/eslint-formatter-pretty .",
        "spec": "jest",
        "test": "cross-env NODE_ENV=test npm run lint && npm run spec && npm run build",
        "version": "npm run build"
    },
    "version": "1.3.5"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module thepiratebay](#apidoc.module.thepiratebay)
1.  [function <span class="apidocSignatureSpan">thepiratebay.</span>convertOrderByObject ()](#apidoc.element.thepiratebay.convertOrderByObject)
1.  [function <span class="apidocSignatureSpan">thepiratebay.</span>getCategories ()](#apidoc.element.thepiratebay.getCategories)
1.  [function <span class="apidocSignatureSpan">thepiratebay.</span>getTorrent (id)](#apidoc.element.thepiratebay.getTorrent)
1.  [function <span class="apidocSignatureSpan">thepiratebay.</span>getTvShow (id)](#apidoc.element.thepiratebay.getTvShow)
1.  [function <span class="apidocSignatureSpan">thepiratebay.</span>recentTorrents ()](#apidoc.element.thepiratebay.recentTorrents)
1.  [function <span class="apidocSignatureSpan">thepiratebay.</span>search ()](#apidoc.element.thepiratebay.search)
1.  [function <span class="apidocSignatureSpan">thepiratebay.</span>topTorrents ()](#apidoc.element.thepiratebay.topTorrents)
1.  [function <span class="apidocSignatureSpan">thepiratebay.</span>userTorrents (username)](#apidoc.element.thepiratebay.userTorrents)
1.  object <span class="apidocSignatureSpan">thepiratebay.</span>Parser
1.  object <span class="apidocSignatureSpan">thepiratebay.</span>default
1.  object <span class="apidocSignatureSpan">thepiratebay.</span>defaultOrder
1.  object <span class="apidocSignatureSpan">thepiratebay.</span>primaryCategoryNumbers
1.  string <span class="apidocSignatureSpan">thepiratebay.</span>baseUrl

#### [module thepiratebay.Parser](#apidoc.module.thepiratebay.Parser)
1.  [function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>_parseTorrentIsTrusted (element)](#apidoc.element.thepiratebay.Parser._parseTorrentIsTrusted)
1.  [function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>_parseTorrentIsVIP (element)](#apidoc.element.thepiratebay.Parser._parseTorrentIsVIP)
1.  [function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>getProxyList ()](#apidoc.element.thepiratebay.Parser.getProxyList)
1.  [function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>isTorrentVerified (element)](#apidoc.element.thepiratebay.Parser.isTorrentVerified)
1.  [function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>parseCategories (categoriesHTML)](#apidoc.element.thepiratebay.Parser.parseCategories)
1.  [function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>parsePage (url, parseCallback)](#apidoc.element.thepiratebay.Parser.parsePage)
1.  [function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>parseResults (resultsHTML)](#apidoc.element.thepiratebay.Parser.parseResults)
1.  [function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>parseTorrentPage (torrentPage)](#apidoc.element.thepiratebay.Parser.parseTorrentPage)
1.  [function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>parseTvShow (tvShowPage)](#apidoc.element.thepiratebay.Parser.parseTvShow)
1.  [function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>parseTvShows (tvShowsPage)](#apidoc.element.thepiratebay.Parser.parseTvShows)

#### [module thepiratebay.default](#apidoc.module.thepiratebay.default)
1.  [function <span class="apidocSignatureSpan">thepiratebay.default.</span>getCategories ()](#apidoc.element.thepiratebay.default.getCategories)
1.  [function <span class="apidocSignatureSpan">thepiratebay.default.</span>getTorrent (id)](#apidoc.element.thepiratebay.default.getTorrent)
1.  [function <span class="apidocSignatureSpan">thepiratebay.default.</span>getTvShow (id)](#apidoc.element.thepiratebay.default.getTvShow)
1.  [function <span class="apidocSignatureSpan">thepiratebay.default.</span>recentTorrents ()](#apidoc.element.thepiratebay.default.recentTorrents)
1.  [function <span class="apidocSignatureSpan">thepiratebay.default.</span>search ()](#apidoc.element.thepiratebay.default.search)
1.  [function <span class="apidocSignatureSpan">thepiratebay.default.</span>topTorrents ()](#apidoc.element.thepiratebay.default.topTorrents)
1.  [function <span class="apidocSignatureSpan">thepiratebay.default.</span>userTorrents (username)](#apidoc.element.thepiratebay.default.userTorrents)



# <a name="apidoc.module.thepiratebay"></a>[module thepiratebay](#apidoc.module.thepiratebay)

#### <a name="apidoc.element.thepiratebay.convertOrderByObject"></a>[function <span class="apidocSignatureSpan">thepiratebay.</span>convertOrderByObject ()](#apidoc.element.thepiratebay.convertOrderByObject)
- description and source-code
```javascript
function convertOrderByObject() {
  var orderByObject = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : defaultOrder;

  var options = [['name', 'desc'], ['name', 'asc'], ['date', 'desc'], ['date', 'asc'], ['size', 'desc'], ['size', 'asc'], ['seeds
', 'desc'], ['seeds', 'asc'], ['leeches', 'desc'], ['leeches', 'asc']];

  // Find the query option
  var option = options.find(function (_option) {
    return _option.includes(orderByObject.orderBy) && _option.includes(orderByObject.sortBy);
  });

  // Get the index of the query option
  var searchNumber = option ? options.indexOf(option) + 1 : undefined;

  if (!searchNumber) throw Error("Can't find option");

  return searchNumber;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thepiratebay.getCategories"></a>[function <span class="apidocSignatureSpan">thepiratebay.</span>getCategories ()](#apidoc.element.thepiratebay.getCategories)
- description and source-code
```javascript
function getCategories() {
  return (0, _Parser.parsePage)(baseUrl + '/recent', _Parser.parseCategories);
}
```
- example usage
```shell
...
sortBy: 'asc'
})
'''

### getCategories
'''javascript
// Gets all available categories on piratebay
PirateBay.getCategories()

/* Returns an array of categories and subcategories
[
{ name: 'Video',
  id: '200',
  subcategories:
   [ { id: '201', name: 'Movies' },
...
```

#### <a name="apidoc.element.thepiratebay.getTorrent"></a>[function <span class="apidocSignatureSpan">thepiratebay.</span>getTorrent (id)](#apidoc.element.thepiratebay.getTorrent)
- description and source-code
```javascript
function getTorrent(id) {
  var url = function () {
    if ((typeof id === 'undefined' ? 'undefined' : (0, _typeof3.default)(id)) === 'object') {
      return id.link;
    }
    return typeof id === 'number' || /^\d+$/.test(id) ? baseUrl + '/torrent/' + id :
    // If id is an object return it's link property. Otherwise,
    // return 'id' itself
    id;
  }();

  return (0, _Parser.parsePage)(url, _Parser.parseTorrentPage);
}
```
- example usage
```shell
...
*/
'''

### getTorrent
'''javascript
// takes an id or a link
PirateBay
.getTorrent('10676856')
.then(results => console.log(results))
.catch(err => console.log(err))

/* Returns a single torrent's description
{
name: 'The Amazing Spider-Man 2 (2014) 1080p BrRip x264 - YIFY',
filesCount: 2,
...
```

#### <a name="apidoc.element.thepiratebay.getTvShow"></a>[function <span class="apidocSignatureSpan">thepiratebay.</span>getTvShow (id)](#apidoc.element.thepiratebay.getTvShow)
- description and source-code
```javascript
function getTvShow(id) {
  return (0, _Parser.parsePage)(baseUrl + '/tv/' + id, _Parser.parseTvShow);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thepiratebay.recentTorrents"></a>[function <span class="apidocSignatureSpan">thepiratebay.</span>recentTorrents ()](#apidoc.element.thepiratebay.recentTorrents)
- description and source-code
```javascript
function recentTorrents() {
  return (0, _Parser.parsePage)(baseUrl + '/recent', _Parser.parseResults);
}
```
- example usage
```shell
...
// returns top 100 torrents for the category '400' aka Games
PirateBay.topTorrents(400)
'''

### recentTorrents
'''javascript
// returns the most recent torrents
PirateBay.recentTorrents()
'''

### userTorrents
'''javascript
// Gets a specific user's torrents
PirateBay.userTorrents('YIFY', {
page: 3,
...
```

#### <a name="apidoc.element.thepiratebay.search"></a>[function <span class="apidocSignatureSpan">thepiratebay.</span>search ()](#apidoc.element.thepiratebay.search)
- description and source-code
```javascript
function search() {
  var title = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : '*';
  var opts = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};

  var convertedCategory = resolveCategory(opts.category, parseInt(searchDefaults.category, 10));

  var castedOptions = (0, _extends3.default)({}, opts, {
    page: opts.page ? castNumberToString(opts.page) : searchDefaults.page,
    category: opts.category ? castNumberToString(convertedCategory) : searchDefaults.category,
    orderby: opts.orderby ? castNumberToString(opts.orderby) : searchDefaults.orderBy
  });

  var _searchDefaults$caste = (0, _extends3.default)({}, searchDefaults, castedOptions),
      page = _searchDefaults$caste.page,
      category = _searchDefaults$caste.category,
      orderBy = _searchDefaults$caste.orderBy,
      sortBy = _searchDefaults$caste.sortBy,
      rest = (0, _objectWithoutProperties3.default)(_searchDefaults$caste, ['page', 'category', 'orderBy', 'sortBy']);

  var orderingNumber = convertOrderByObject({ orderBy: orderBy, sortBy: sortBy });

  var url = baseUrl + '/s/?' + _querystring2.default.stringify({
    q: title,
    category: category,
    page: page,
    orderby: orderingNumber
  });

  return (0, _Parser.parsePage)(url, _Parser.parseResults, rest.filter);
}
```
- example usage
```shell
...
const PirateBay = require('thepiratebay')
'''
All methods are asynchronous!
You can use promises, ES6 generators, or async/await

Using promises:
'''javascript
PirateBay.search('Game of Thrones', {
  category: 205
})
.then(results => console.log(results))
.catch(err => console.log(err))
'''

Using ES7 async/await (requires babel)
...
```

#### <a name="apidoc.element.thepiratebay.topTorrents"></a>[function <span class="apidocSignatureSpan">thepiratebay.</span>topTorrents ()](#apidoc.element.thepiratebay.topTorrents)
- description and source-code
```javascript
function topTorrents() {
  var category = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : 'all';

  var castedCategory = void 0;

  // Check if category is number and can be casted
  if (parseInt(category, 10)) {
    castedCategory = castNumberToString(category);
  }

  return (0, _Parser.parsePage)(baseUrl + '/top/' + (castedCategory || category), _Parser.parseResults);
}
```
- example usage
```shell
...
}
*/
'''

### topTorrents
'''javascript
// returns top 100 torrents
PirateBay.topTorrents()

// returns top 100 torrents for the category '400' aka Games
PirateBay.topTorrents(400)
'''

### recentTorrents
'''javascript
...
```

#### <a name="apidoc.element.thepiratebay.userTorrents"></a>[function <span class="apidocSignatureSpan">thepiratebay.</span>userTorrents (username)](#apidoc.element.thepiratebay.userTorrents)
- description and source-code
```javascript
function userTorrents(username) {
  var opts = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};
  var orderby = opts.orderby;


  // Determine orderingNumber given orderBy and sortBy
  if (opts.sortBy || opts.orderBy) {
    orderby = convertOrderByObject({
      sortBy: opts.sortBy || 'desc',
      orderBy: opts.orderBy || 'seeds'
    });
  }

  var query = baseUrl + '/user/' + username + '/?' + _querystring2.default.stringify({
    page: opts.page ? castNumberToString(opts.page) : '0',
    orderby: orderby || '99'
  });

  return (0, _Parser.parsePage)(query, _Parser.parseResults);
}
```
- example usage
```shell
...
// returns the most recent torrents
PirateBay.recentTorrents()
'''

### userTorrents
'''javascript
// Gets a specific user's torrents
PirateBay.userTorrents('YIFY', {
  page: 3,
  orderBy: 'name',
  sortBy: 'asc'
})
'''

### getCategories
...
```



# <a name="apidoc.module.thepiratebay.Parser"></a>[module thepiratebay.Parser](#apidoc.module.thepiratebay.Parser)

#### <a name="apidoc.element.thepiratebay.Parser._parseTorrentIsTrusted"></a>[function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>_parseTorrentIsTrusted (element)](#apidoc.element.thepiratebay.Parser._parseTorrentIsTrusted)
- description and source-code
```javascript
function _parseTorrentIsTrusted(element) {
  return element.find('img[title="Trusted"]').attr('title') === 'Trusted';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thepiratebay.Parser._parseTorrentIsVIP"></a>[function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>_parseTorrentIsVIP (element)](#apidoc.element.thepiratebay.Parser._parseTorrentIsVIP)
- description and source-code
```javascript
function _parseTorrentIsVIP(element) {
  return element.find('img[title="VIP"]').attr('title') === 'VIP';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thepiratebay.Parser.getProxyList"></a>[function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>getProxyList ()](#apidoc.element.thepiratebay.Parser.getProxyList)
- description and source-code
```javascript
function getProxyList() {
  return _ref.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thepiratebay.Parser.isTorrentVerified"></a>[function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>isTorrentVerified (element)](#apidoc.element.thepiratebay.Parser.isTorrentVerified)
- description and source-code
```javascript
function isTorrentVerified(element) {
  return _parseTorrentIsVIP(element) || _parseTorrentIsTrusted(element);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thepiratebay.Parser.parseCategories"></a>[function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>parseCategories (categoriesHTML)](#apidoc.element.thepiratebay.Parser.parseCategories)
- description and source-code
```javascript
function parseCategories(categoriesHTML) {
  var $ = _cheerio2.default.load(categoriesHTML);
  var categoriesContainer = $('select#category optgroup');
  var currentCategoryId = 0;

  var categories = categoriesContainer.map(function getElements() {
    currentCategoryId += 100;

    var category = {
      name: $(this).attr('label'),
      id: '' + currentCategoryId,
      subcategories: []
    };

    $(this).find('option').each(function getSubcategory() {
      var subcategory = {
        id: $(this).attr('value'),
        name: $(this).text()
      };

      return category.subcategories.push(subcategory);
    });

    return category;
  });

  return categories.get();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thepiratebay.Parser.parsePage"></a>[function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>parsePage (url, parseCallback)](#apidoc.element.thepiratebay.Parser.parsePage)
- description and source-code
```javascript
function parsePage(url, parseCallback) {
  var _this = this;

  var filter = arguments.length > 2 && arguments[2] !== undefined ? arguments[2] : {};

  var attempt = function () {
    var _ref2 = (0, _asyncToGenerator3.default)(_regenerator2.default.mark(function _callee2(error) {
      var proxyUrls, requests, abandonFailedResponses, race;
      return _regenerator2.default.wrap(function _callee2$(_context2) {
        while (1) {
          switch (_context2.prev = _context2.next) {
            case 0:
              if (error) console.log(error);

              proxyUrls = ['https://thepiratebay.org', 'https://thepiratebay.se', 'https://pirateproxy.one', 'https://ahoy.one'];
              requests = proxyUrls.map(function (_url) {
                return new _urlParse2.default(url).set('hostname', new _urlParse2.default(_url).hostname).href;
              }).map(function (_url) {
                return (0, _isomorphicFetch2.default)(_url, { mode: 'no-cors' }).then(function (response) {
                  return response.text();
                }).then(function (body) {
                  return body.includes('502: Bad gateway') || body.includes('Database maintenance') ? _promise2.default.reject('
Database maintenance or 502 error') : _promise2.default.resolve(body);
                });
              });

              abandonFailedResponses = function abandonFailedResponses(index) {
                var p = requests.splice(index, 1)[0];
                p.catch();
              };

              race = function race() {
                if (requests.length < 1) {
                  return _promise2.default.reject('None of the proxy requests were successful');
                }
                var indexedRequests = requests.map(function (p, index) {
                  return p.catch(function () {
                    throw index;
                  });
                });
                return _promise2.default.race(indexedRequests).catch(function (index) {
                  abandonFailedResponses(index);
                  return race(requests);
                });
              };

              return _context2.abrupt('return', race(requests));

            case 6:
            case 'end':
              return _context2.stop();
          }
        }
      }, _callee2, _this);
    }));

    return function attempt(_x2) {
      return _ref2.apply(this, arguments);
    };
  }();

  return attempt().catch(function () {
    return attempt('Failed, retrying');
  }).then(function (response) {
    return parseCallback(response, filter);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thepiratebay.Parser.parseResults"></a>[function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>parseResults (resultsHTML)](#apidoc.element.thepiratebay.Parser.parseResults)
- description and source-code
```javascript
function parseResults(resultsHTML) {
  var filter = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};

  var $ = _cheerio2.default.load(resultsHTML);
  var rawResults = $('table#searchResult tr:has(a.detLink)');

  var results = rawResults.map(function getRawResults() {
    var name = $(this).find('a.detLink').text();
    var uploadDate = $(this).find('font').text().match(/Uploaded\s(?:<b>)?(.+?)(?:<\/b>)?,/)[1];
    var size = $(this).find('font').text().match(/Size (.+?),/)[1];

    var seeders = $(this).find('td[align="right"]').first().text();
    var leechers = $(this).find('td[align="right"]').next().text();
    var relativeLink = $(this).find('div.detName a').attr('href');
    var link = _PirateBay.baseUrl + relativeLink;
    var id = String(parseInt(/^\/torrent\/(\d+)/.exec(relativeLink)[1], 10));
    var magnetLink = $(this).find('a[title="Download this torrent using magnet"]').attr('href');
    var uploader = $(this).find('font .detDesc').text();
    var uploaderLink = _PirateBay.baseUrl + $(this).find('font a').attr('href');
    var verified = isTorrentVerified($(this));

    var category = {
      id: $(this).find('center a').first().attr('href').match(/\/browse\/(\d+)/)[1],
      name: $(this).find('center a').first().text()
    };

    var subcategory = {
      id: $(this).find('center a').last().attr('href').match(/\/browse\/(\d+)/)[1],
      name: $(this).find('center a').last().text()
    };

    return {
      id: id,
      name: name,
      size: size,
      link: link,
      category: category,
      seeders: seeders,
      leechers: leechers,
      uploadDate: uploadDate,
      magnetLink: magnetLink,
      subcategory: subcategory,
      uploader: uploader,
      verified: verified,
      uploaderLink: uploaderLink
    };
  });

  var parsedResultsArray = results.get().filter(function (result) {
    return !result.uploaderLink.includes('undefined');
  });

  return filter.verified === true ? parsedResultsArray.filter(function (result) {
    return result.verified === true;
  }) : parsedResultsArray;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thepiratebay.Parser.parseTorrentPage"></a>[function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>parseTorrentPage (torrentPage)](#apidoc.element.thepiratebay.Parser.parseTorrentPage)
- description and source-code
```javascript
function parseTorrentPage(torrentPage) {
  var $ = _cheerio2.default.load(torrentPage);
  var name = $('#title').text().trim();

  var size = $('dt:contains(Size:) + dd').text().trim();
  var uploadDate = $('dt:contains(Uploaded:) + dd').text().trim();
  var uploader = $('dt:contains(By:) + dd').text().trim();
  var uploaderLink = _PirateBay.baseUrl + $('dt:contains(By:) + dd a').attr('href');
  var seeders = $('dt:contains(Seeders:) + dd').text().trim();
  var leechers = $('dt:contains(Leechers:) + dd').text().trim();
  var id = $('input[name=id]').attr('value');
  var link = _PirateBay.baseUrl + '/torrent/' + id;
  var magnetLink = $('a[title="Get this torrent"]').attr('href');
  var description = $('div.nfo').text().trim();

  return {
    category: '',
    name: name,
    size: size,
    seeders: seeders,
    leechers: leechers,
    uploadDate: uploadDate,
    magnetLink: magnetLink,
    link: link,
    id: id,
    description: description,
    uploader: uploader,
    uploaderLink: uploaderLink
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thepiratebay.Parser.parseTvShow"></a>[function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>parseTvShow (tvShowPage)](#apidoc.element.thepiratebay.Parser.parseTvShow)
- description and source-code
```javascript
function parseTvShow(tvShowPage) {
  var _this2 = this;

  var $ = _cheerio2.default.load(tvShowPage);
  var seasons = $('dt a').map(function () {
    return $(_this2).text();
  }).get();
  var rawLinks = $('dd');

  var torrents = rawLinks.map(function (element) {
    return $(_this2).find('a').map(function () {
      return {
        title: element.text(),
        link: _PirateBay.baseUrl + element.attr('href'),
        id: element.attr('href').match(/\/torrent\/(\d+)/)[1]
      };
    }).get();
  });

  return seasons.map(function (season, index) {
    return {
      title: season,
      torrents: torrents[index]
    };
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thepiratebay.Parser.parseTvShows"></a>[function <span class="apidocSignatureSpan">thepiratebay.Parser.</span>parseTvShows (tvShowsPage)](#apidoc.element.thepiratebay.Parser.parseTvShows)
- description and source-code
```javascript
function parseTvShows(tvShowsPage) {
  var $ = _cheerio2.default.load(tvShowsPage);
  var rawTitles = $('dt a');
  var series = rawTitles.map(function (element) {
    return {
      title: element.text(),
      id: element.attr('href').match(/\/tv\/(\d+)/)[1]
    };
  }).get();

  var rawSeasons = $('dd');
  var seasons = rawSeasons.map(function (element) {
    return element.find('a').text().match(/S\d+/g);
  });

  return series.map(function (s, index) {
    return {
      title: s.title,
      id: s.id,
      seasons: seasons[index]
    };
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.thepiratebay.default"></a>[module thepiratebay.default](#apidoc.module.thepiratebay.default)

#### <a name="apidoc.element.thepiratebay.default.getCategories"></a>[function <span class="apidocSignatureSpan">thepiratebay.default.</span>getCategories ()](#apidoc.element.thepiratebay.default.getCategories)
- description and source-code
```javascript
function getCategories() {
  return (0, _Parser.parsePage)(baseUrl + '/recent', _Parser.parseCategories);
}
```
- example usage
```shell
...
sortBy: 'asc'
})
'''

### getCategories
'''javascript
// Gets all available categories on piratebay
PirateBay.getCategories()

/* Returns an array of categories and subcategories
[
{ name: 'Video',
  id: '200',
  subcategories:
   [ { id: '201', name: 'Movies' },
...
```

#### <a name="apidoc.element.thepiratebay.default.getTorrent"></a>[function <span class="apidocSignatureSpan">thepiratebay.default.</span>getTorrent (id)](#apidoc.element.thepiratebay.default.getTorrent)
- description and source-code
```javascript
function getTorrent(id) {
  var url = function () {
    if ((typeof id === 'undefined' ? 'undefined' : (0, _typeof3.default)(id)) === 'object') {
      return id.link;
    }
    return typeof id === 'number' || /^\d+$/.test(id) ? baseUrl + '/torrent/' + id :
    // If id is an object return it's link property. Otherwise,
    // return 'id' itself
    id;
  }();

  return (0, _Parser.parsePage)(url, _Parser.parseTorrentPage);
}
```
- example usage
```shell
...
*/
'''

### getTorrent
'''javascript
// takes an id or a link
PirateBay
.getTorrent('10676856')
.then(results => console.log(results))
.catch(err => console.log(err))

/* Returns a single torrent's description
{
name: 'The Amazing Spider-Man 2 (2014) 1080p BrRip x264 - YIFY',
filesCount: 2,
...
```

#### <a name="apidoc.element.thepiratebay.default.getTvShow"></a>[function <span class="apidocSignatureSpan">thepiratebay.default.</span>getTvShow (id)](#apidoc.element.thepiratebay.default.getTvShow)
- description and source-code
```javascript
function getTvShow(id) {
  return (0, _Parser.parsePage)(baseUrl + '/tv/' + id, _Parser.parseTvShow);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.thepiratebay.default.recentTorrents"></a>[function <span class="apidocSignatureSpan">thepiratebay.default.</span>recentTorrents ()](#apidoc.element.thepiratebay.default.recentTorrents)
- description and source-code
```javascript
function recentTorrents() {
  return (0, _Parser.parsePage)(baseUrl + '/recent', _Parser.parseResults);
}
```
- example usage
```shell
...
// returns top 100 torrents for the category '400' aka Games
PirateBay.topTorrents(400)
'''

### recentTorrents
'''javascript
// returns the most recent torrents
PirateBay.recentTorrents()
'''

### userTorrents
'''javascript
// Gets a specific user's torrents
PirateBay.userTorrents('YIFY', {
page: 3,
...
```

#### <a name="apidoc.element.thepiratebay.default.search"></a>[function <span class="apidocSignatureSpan">thepiratebay.default.</span>search ()](#apidoc.element.thepiratebay.default.search)
- description and source-code
```javascript
function search() {
  var title = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : '*';
  var opts = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};

  var convertedCategory = resolveCategory(opts.category, parseInt(searchDefaults.category, 10));

  var castedOptions = (0, _extends3.default)({}, opts, {
    page: opts.page ? castNumberToString(opts.page) : searchDefaults.page,
    category: opts.category ? castNumberToString(convertedCategory) : searchDefaults.category,
    orderby: opts.orderby ? castNumberToString(opts.orderby) : searchDefaults.orderBy
  });

  var _searchDefaults$caste = (0, _extends3.default)({}, searchDefaults, castedOptions),
      page = _searchDefaults$caste.page,
      category = _searchDefaults$caste.category,
      orderBy = _searchDefaults$caste.orderBy,
      sortBy = _searchDefaults$caste.sortBy,
      rest = (0, _objectWithoutProperties3.default)(_searchDefaults$caste, ['page', 'category', 'orderBy', 'sortBy']);

  var orderingNumber = convertOrderByObject({ orderBy: orderBy, sortBy: sortBy });

  var url = baseUrl + '/s/?' + _querystring2.default.stringify({
    q: title,
    category: category,
    page: page,
    orderby: orderingNumber
  });

  return (0, _Parser.parsePage)(url, _Parser.parseResults, rest.filter);
}
```
- example usage
```shell
...
const PirateBay = require('thepiratebay')
'''
All methods are asynchronous!
You can use promises, ES6 generators, or async/await

Using promises:
'''javascript
PirateBay.search('Game of Thrones', {
  category: 205
})
.then(results => console.log(results))
.catch(err => console.log(err))
'''

Using ES7 async/await (requires babel)
...
```

#### <a name="apidoc.element.thepiratebay.default.topTorrents"></a>[function <span class="apidocSignatureSpan">thepiratebay.default.</span>topTorrents ()](#apidoc.element.thepiratebay.default.topTorrents)
- description and source-code
```javascript
function topTorrents() {
  var category = arguments.length > 0 && arguments[0] !== undefined ? arguments[0] : 'all';

  var castedCategory = void 0;

  // Check if category is number and can be casted
  if (parseInt(category, 10)) {
    castedCategory = castNumberToString(category);
  }

  return (0, _Parser.parsePage)(baseUrl + '/top/' + (castedCategory || category), _Parser.parseResults);
}
```
- example usage
```shell
...
}
*/
'''

### topTorrents
'''javascript
// returns top 100 torrents
PirateBay.topTorrents()

// returns top 100 torrents for the category '400' aka Games
PirateBay.topTorrents(400)
'''

### recentTorrents
'''javascript
...
```

#### <a name="apidoc.element.thepiratebay.default.userTorrents"></a>[function <span class="apidocSignatureSpan">thepiratebay.default.</span>userTorrents (username)](#apidoc.element.thepiratebay.default.userTorrents)
- description and source-code
```javascript
function userTorrents(username) {
  var opts = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : {};
  var orderby = opts.orderby;


  // Determine orderingNumber given orderBy and sortBy
  if (opts.sortBy || opts.orderBy) {
    orderby = convertOrderByObject({
      sortBy: opts.sortBy || 'desc',
      orderBy: opts.orderBy || 'seeds'
    });
  }

  var query = baseUrl + '/user/' + username + '/?' + _querystring2.default.stringify({
    page: opts.page ? castNumberToString(opts.page) : '0',
    orderby: orderby || '99'
  });

  return (0, _Parser.parsePage)(query, _Parser.parseResults);
}
```
- example usage
```shell
...
// returns the most recent torrents
PirateBay.recentTorrents()
'''

### userTorrents
'''javascript
// Gets a specific user's torrents
PirateBay.userTorrents('YIFY', {
  page: 3,
  orderBy: 'name',
  sortBy: 'asc'
})
'''

### getCategories
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
