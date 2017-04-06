# api documentation for  [dav (v1.7.8)](https://github.com/gaye/dav#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-dav.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-dav) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-dav.svg)](https://travis-ci.org/npmdoc/node-npmdoc-dav)
#### WebDAV, CalDAV, and CardDAV client for nodejs and the browser

[![NPM](https://nodei.co/npm/dav.png?downloads=true)](https://www.npmjs.com/package/dav)

[![apidoc](https://npmdoc.github.io/node-npmdoc-dav/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-dav_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-dav/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-dav/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-dav/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Gareth Aye [:gaye]",
        "email": "gaye@mozilla.com"
    },
    "bugs": {
        "url": "https://github.com/gaye/dav/issues"
    },
    "dependencies": {
        "co": "^4.6.0",
        "xmldom": "^0.1.19",
        "xmlhttprequest": "^1.7.0"
    },
    "description": "WebDAV, CalDAV, and CardDAV client for nodejs and the browser",
    "devDependencies": {
        "babel": "^5.8.23",
        "browserify": "^11.0.1",
        "chai": "^3.2.0",
        "doctoc": "^0.15.0",
        "mocha": "^2.3.2",
        "nock": "^2.10.0",
        "sinon": "^1.16.1",
        "tcp-port-used": "^0.1.2",
        "uglify-js": "^2.4.24"
    },
    "directories": {},
    "dist": {
        "shasum": "f664031222e1af1bc7cd2fc183c2ecea1781c74a",
        "tarball": "https://registry.npmjs.org/dav/-/dav-1.7.8.tgz"
    },
    "gitHead": "a4cb4490ea68d646034f3a0e61e86744889e19aa",
    "homepage": "https://github.com/gaye/dav#readme",
    "keywords": [
        "address book",
        "calendar",
        "contacts",
        "dav",
        "caldav",
        "carddav",
        "webdav",
        "ical",
        "vcard",
        "sync",
        "rfc 4791",
        "rfc 6352",
        "rfc 6578"
    ],
    "license": "MPL-2.0",
    "main": "./dav.js",
    "maintainers": [
        {
            "name": "gaye",
            "email": "gareth.aye@gmail.com"
        }
    ],
    "name": "dav",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/gaye/dav.git"
    },
    "scripts": {
        "test": "make test"
    },
    "version": "1.7.8"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module dav](#apidoc.module.dav)
1.  [function <span class="apidocSignatureSpan">dav.</span>Account (options)](#apidoc.element.dav.Account)
1.  [function <span class="apidocSignatureSpan">dav.</span>AddressBook (options)](#apidoc.element.dav.AddressBook)
1.  [function <span class="apidocSignatureSpan">dav.</span>Calendar (options)](#apidoc.element.dav.Calendar)
1.  [function <span class="apidocSignatureSpan">dav.</span>CalendarObject (options)](#apidoc.element.dav.CalendarObject)
1.  [function <span class="apidocSignatureSpan">dav.</span>Client (xhr)](#apidoc.element.dav.Client)
1.  [function <span class="apidocSignatureSpan">dav.</span>Credentials (options)](#apidoc.element.dav.Credentials)
1.  [function <span class="apidocSignatureSpan">dav.</span>DAVCollection (options)](#apidoc.element.dav.DAVCollection)
1.  [function <span class="apidocSignatureSpan">dav.</span>DAVObject (options)](#apidoc.element.dav.DAVObject)
1.  [function <span class="apidocSignatureSpan">dav.</span>Request ()](#apidoc.element.dav.Request)
1.  [function <span class="apidocSignatureSpan">dav.</span>Sandbox ()](#apidoc.element.dav.Sandbox)
1.  [function <span class="apidocSignatureSpan">dav.</span>VCard (options)](#apidoc.element.dav.VCard)
1.  [function <span class="apidocSignatureSpan">dav.</span>createAccount ()](#apidoc.element.dav.createAccount)
1.  [function <span class="apidocSignatureSpan">dav.</span>createCalendarObject (calendar, options)](#apidoc.element.dav.createCalendarObject)
1.  [function <span class="apidocSignatureSpan">dav.</span>createCard (addressBook, options)](#apidoc.element.dav.createCard)
1.  [function <span class="apidocSignatureSpan">dav.</span>createSandbox ()](#apidoc.element.dav.createSandbox)
1.  [function <span class="apidocSignatureSpan">dav.</span>debug (topic)](#apidoc.element.dav.debug)
1.  [function <span class="apidocSignatureSpan">dav.</span>deleteCalendarObject (calendarObject, options)](#apidoc.element.dav.deleteCalendarObject)
1.  [function <span class="apidocSignatureSpan">dav.</span>deleteCard (card, options)](#apidoc.element.dav.deleteCard)
1.  [function <span class="apidocSignatureSpan">dav.</span>listAddressBooks ()](#apidoc.element.dav.listAddressBooks)
1.  [function <span class="apidocSignatureSpan">dav.</span>listCalendarObjects ()](#apidoc.element.dav.listCalendarObjects)
1.  [function <span class="apidocSignatureSpan">dav.</span>listCalendars ()](#apidoc.element.dav.listCalendars)
1.  [function <span class="apidocSignatureSpan">dav.</span>listVCards ()](#apidoc.element.dav.listVCards)
1.  [function <span class="apidocSignatureSpan">dav.</span>syncAddressBook (addressBook, options)](#apidoc.element.dav.syncAddressBook)
1.  [function <span class="apidocSignatureSpan">dav.</span>syncCaldavAccount ()](#apidoc.element.dav.syncCaldavAccount)
1.  [function <span class="apidocSignatureSpan">dav.</span>syncCalendar (calendar, options)](#apidoc.element.dav.syncCalendar)
1.  [function <span class="apidocSignatureSpan">dav.</span>syncCarddavAccount ()](#apidoc.element.dav.syncCarddavAccount)
1.  [function <span class="apidocSignatureSpan">dav.</span>updateCalendarObject (calendarObject, options)](#apidoc.element.dav.updateCalendarObject)
1.  [function <span class="apidocSignatureSpan">dav.</span>updateCard (card, options)](#apidoc.element.dav.updateCard)
1.  object <span class="apidocSignatureSpan">dav.</span>ns
1.  object <span class="apidocSignatureSpan">dav.</span>request
1.  object <span class="apidocSignatureSpan">dav.</span>transport
1.  string <span class="apidocSignatureSpan">dav.</span>version

#### [module dav.createAccount](#apidoc.module.dav.createAccount)
1.  [function <span class="apidocSignatureSpan">dav.</span>createAccount ()](#apidoc.element.dav.createAccount.createAccount)
1.  [function <span class="apidocSignatureSpan">dav.createAccount.</span>__generatorFunction__ (options)](#apidoc.element.dav.createAccount.__generatorFunction__)

#### [module dav.listAddressBooks](#apidoc.module.dav.listAddressBooks)
1.  [function <span class="apidocSignatureSpan">dav.</span>listAddressBooks ()](#apidoc.element.dav.listAddressBooks.listAddressBooks)
1.  [function <span class="apidocSignatureSpan">dav.listAddressBooks.</span>__generatorFunction__ (account, options)](#apidoc.element.dav.listAddressBooks.__generatorFunction__)

#### [module dav.listCalendarObjects](#apidoc.module.dav.listCalendarObjects)
1.  [function <span class="apidocSignatureSpan">dav.</span>listCalendarObjects ()](#apidoc.element.dav.listCalendarObjects.listCalendarObjects)
1.  [function <span class="apidocSignatureSpan">dav.listCalendarObjects.</span>__generatorFunction__ (calendar, options)](#apidoc.element.dav.listCalendarObjects.__generatorFunction__)

#### [module dav.listCalendars](#apidoc.module.dav.listCalendars)
1.  [function <span class="apidocSignatureSpan">dav.</span>listCalendars ()](#apidoc.element.dav.listCalendars.listCalendars)
1.  [function <span class="apidocSignatureSpan">dav.listCalendars.</span>__generatorFunction__ (account, options)](#apidoc.element.dav.listCalendars.__generatorFunction__)

#### [module dav.listVCards](#apidoc.module.dav.listVCards)
1.  [function <span class="apidocSignatureSpan">dav.</span>listVCards ()](#apidoc.element.dav.listVCards.listVCards)
1.  [function <span class="apidocSignatureSpan">dav.listVCards.</span>__generatorFunction__ (addressBook, options)](#apidoc.element.dav.listVCards.__generatorFunction__)

#### [module dav.request](#apidoc.module.dav.request)
1.  [function <span class="apidocSignatureSpan">dav.request.</span>Request ()](#apidoc.element.dav.request.Request)
1.  [function <span class="apidocSignatureSpan">dav.request.</span>addressBookQuery (options)](#apidoc.element.dav.request.addressBookQuery)
1.  [function <span class="apidocSignatureSpan">dav.request.</span>basic (options)](#apidoc.element.dav.request.basic)
1.  [function <span class="apidocSignatureSpan">dav.request.</span>calendarQuery (options)](#apidoc.element.dav.request.calendarQuery)
1.  [function <span class="apidocSignatureSpan">dav.request.</span>collectionQuery (requestData, options)](#apidoc.element.dav.request.collectionQuery)
1.  [function <span class="apidocSignatureSpan">dav.request.</span>getProps (propstats)](#apidoc.element.dav.request.getProps)
1.  [function <span class="apidocSignatureSpan">dav.request.</span>mergeProps (props)](#apidoc.element.dav.request.mergeProps)
1.  [function <span class="apidocSignatureSpan">dav.request.</span>propfind (options)](#apidoc.element.dav.request.propfind)
1.  [function <span class="apidocSignatureSpan">dav.request.</span>setRequestHeaders (request, options)](#apidoc.element.dav.request.setRequestHeaders)
1.  [function <span class="apidocSignatureSpan">dav.request.</span>syncCollection (options)](#apidoc.element.dav.request.syncCollection)

#### [module dav.syncCaldavAccount](#apidoc.module.dav.syncCaldavAccount)
1.  [function <span class="apidocSignatureSpan">dav.</span>syncCaldavAccount ()](#apidoc.element.dav.syncCaldavAccount.syncCaldavAccount)
1.  [function <span class="apidocSignatureSpan">dav.syncCaldavAccount.</span>__generatorFunction__ (account)](#apidoc.element.dav.syncCaldavAccount.__generatorFunction__)

#### [module dav.syncCarddavAccount](#apidoc.module.dav.syncCarddavAccount)
1.  [function <span class="apidocSignatureSpan">dav.</span>syncCarddavAccount ()](#apidoc.element.dav.syncCarddavAccount.syncCarddavAccount)
1.  [function <span class="apidocSignatureSpan">dav.syncCarddavAccount.</span>__generatorFunction__ (account)](#apidoc.element.dav.syncCarddavAccount.__generatorFunction__)

#### [module dav.transport](#apidoc.module.dav.transport)
1.  [function <span class="apidocSignatureSpan">dav.transport.</span>Basic (credentials)](#apidoc.element.dav.transport.Basic)
1.  [function <span class="apidocSignatureSpan">dav.transport.</span>OAuth2 (credentials)](#apidoc.element.dav.transport.OAuth2)
1.  [function <span class="apidocSignatureSpan">dav.transport.</span>Transport (credentials)](#apidoc.element.dav.transport.Transport)



# <a name="apidoc.module.dav"></a>[module dav](#apidoc.module.dav)

#### <a name="apidoc.element.dav.Account"></a>[function <span class="apidocSignatureSpan">dav.</span>Account (options)](#apidoc.element.dav.Account)
- description and source-code
```javascript
function Account(options) {
  _classCallCheck(this, Account);

  Object.assign(this, {
    server: null,
    credentials: null,
    rootUrl: null,
    principalUrl: null,
    homeUrl: null,
    calendars: null,
    addressBooks: null
  }, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.AddressBook"></a>[function <span class="apidocSignatureSpan">dav.</span>AddressBook (options)](#apidoc.element.dav.AddressBook)
- description and source-code
```javascript
function AddressBook(options) {
  _classCallCheck(this, AddressBook);

  _get(Object.getPrototypeOf(AddressBook.prototype), "constructor", this).call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.Calendar"></a>[function <span class="apidocSignatureSpan">dav.</span>Calendar (options)](#apidoc.element.dav.Calendar)
- description and source-code
```javascript
function Calendar(options) {
  _classCallCheck(this, Calendar);

  _get(Object.getPrototypeOf(Calendar.prototype), "constructor", this).call(this, options);
  Object.assign(this, {
    components: null,
    timezone: null
  }, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.CalendarObject"></a>[function <span class="apidocSignatureSpan">dav.</span>CalendarObject (options)](#apidoc.element.dav.CalendarObject)
- description and source-code
```javascript
function CalendarObject(options) {
  _classCallCheck(this, CalendarObject);

  _get(Object.getPrototypeOf(CalendarObject.prototype), "constructor", this).call(this, options);
  Object.assign(this, {
    calendar: null,
    calendarData: null
  }, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.Client"></a>[function <span class="apidocSignatureSpan">dav.</span>Client (xhr)](#apidoc.element.dav.Client)
- description and source-code
```javascript
function Client(xhr) {
  var options = arguments.length <= 1 || arguments[1] === undefined ? {} : arguments[1];

  _classCallCheck(this, Client);

  this.xhr = xhr;
  Object.assign(this, options);

  // Expose internal modules for unit testing
  this._accounts = accounts;
  this._calendars = calendars;
  this._contacts = contacts;
}
```
- example usage
```shell
...
  - [request](#request)
    - [dav.request.addressBookQuery(options)](#davrequestaddressbookqueryoptions)
    - [dav.request.basic(options)](#davrequestbasicoptions)
    - [dav.request.calendarQuery(options)](#davrequestcalendarqueryoptions)
    - [dav.request.propfind(options)](#davrequestpropfindoptions)
    - [dav.request.syncCollection(options)](#davrequestsynccollectionoptions)
  - [Client](#client)
    - [dav.Client(xhr, options)](#davclientxhr-options)
      - [dav.Client.send(req, options)](#davclientsendreq-options)
  - [etc](#etc)
    - [dav.ns](#davns)
  - [Example Usage](#example-usage)
    - [Using the lower-level webdav request api](#using-the-lower-level-webdav-request-api)
- [Debugging](#debugging)
...
```

#### <a name="apidoc.element.dav.Credentials"></a>[function <span class="apidocSignatureSpan">dav.</span>Credentials (options)](#apidoc.element.dav.Credentials)
- description and source-code
```javascript
function Credentials(options) {
  _classCallCheck(this, Credentials);

  Object.assign(this, {
    username: null,
    password: null,
    clientId: null,
    clientSecret: null,
    authorizationCode: null,
    redirectUrl: null,
    tokenUrl: null,
    accessToken: null,
    refreshToken: null,
    expiration: null
  }, options);
}
```
- example usage
```shell
...

### Example Usage

'''js
var dav = require('dav');

var xhr = new dav.transport.Basic(
  new dav.Credentials({
    username: 'xxx',
    password: 'xxx'
  })
);

dav.createAccount({ server: 'http://dav.example.com', xhr: xhr })
.then(function(account) {
...
```

#### <a name="apidoc.element.dav.DAVCollection"></a>[function <span class="apidocSignatureSpan">dav.</span>DAVCollection (options)](#apidoc.element.dav.DAVCollection)
- description and source-code
```javascript
function DAVCollection(options) {
  _classCallCheck(this, DAVCollection);

  Object.assign(this, {
    data: null,
    objects: null,
    account: null,
    ctag: null,
    description: null,
    displayName: null,
    reports: null,
    resourcetype: null,
    syncToken: null,
    url: null
  }, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.DAVObject"></a>[function <span class="apidocSignatureSpan">dav.</span>DAVObject (options)](#apidoc.element.dav.DAVObject)
- description and source-code
```javascript
function DAVObject(options) {
  _classCallCheck(this, DAVObject);

  Object.assign(this, {
    data: null,
    etag: null,
    url: null
  }, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.Request"></a>[function <span class="apidocSignatureSpan">dav.</span>Request ()](#apidoc.element.dav.Request)
- description and source-code
```javascript
function Request() {
  var options = arguments.length <= 0 || arguments[0] === undefined ? {} : arguments[0];

  _classCallCheck(this, Request);

  Object.assign(this, {
    method: null,
    requestData: null,
    transformRequest: null,
    transformResponse: null,
    onerror: null
  }, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.Sandbox"></a>[function <span class="apidocSignatureSpan">dav.</span>Sandbox ()](#apidoc.element.dav.Sandbox)
- description and source-code
```javascript
function Sandbox() {
  _classCallCheck(this, Sandbox);

  this.requestList = [];
}
```
- example usage
```shell
...
- [contacts](#contacts)
  - [dav.createCard(addressBook, options)](#davcreatecardaddressbook-options)
  - [dav.updateCard(card, options)](#davupdatecardcard-options)
  - [dav.deleteCard(card, options)](#davdeletecardcard-options)
  - [dav.syncAddressBook(addressBook, options)](#davsyncaddressbookaddressbook-options)
  - [dav.syncCarddavAccount(account, options)](#davsynccarddavaccountaccount-options)
- [sandbox](#sandbox)
  - [dav.Sandbox()](#davsandbox)
- [transport](#transport)
  - [dav.transport.Basic(credentials)](#davtransportbasiccredentials)
    - [dav.transport.Basic.send(request, options)](#davtransportbasicsendrequest-options)
  - [dav.transport.OAuth2(credentials)](#davtransportoauth2credentials)
    - [dav.transport.OAuth2.send(request, options)](#davtransportoauth2sendrequest-options)
- [request](#request)
  - [dav.request.addressBookQuery(options)](#davrequestaddressbookqueryoptions)
...
```

#### <a name="apidoc.element.dav.VCard"></a>[function <span class="apidocSignatureSpan">dav.</span>VCard (options)](#apidoc.element.dav.VCard)
- description and source-code
```javascript
function VCard(options) {
  _classCallCheck(this, VCard);

  _get(Object.getPrototypeOf(VCard.prototype), "constructor", this).call(this, options);
  Object.assign(this, {
    addressBook: null,
    addressData: null
  }, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.createAccount"></a>[function <span class="apidocSignatureSpan">dav.</span>createAccount ()](#apidoc.element.dav.createAccount)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
...

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](http://doctoc.herokuapp.com/)*

- [API](#api)
- [accounts](#accounts)
  - [dav.createAccount(options)](#davcreateaccountoptions)
- [calendars](#calendars)
  - [dav.createCalendarObject(calendar, options)](#davcreatecalendarobjectcalendar-options)
  - [dav.updateCalendarObject(calendarObject, options)](#davupdatecalendarobjectcalendarobject-options)
  - [dav.deleteCalendarObject(calendarObject, options)](#davdeletecalendarobjectcalendarobject-options)
  - [dav.syncCalendar(calendar, options)](#davsynccalendarcalendar-options)
  - [dav.syncCaldavAccount(account, options)](#davsynccaldavaccountaccount-options)
- [contacts](#contacts)
...
```

#### <a name="apidoc.element.dav.createCalendarObject"></a>[function <span class="apidocSignatureSpan">dav.</span>createCalendarObject (calendar, options)](#apidoc.element.dav.createCalendarObject)
- description and source-code
```javascript
function createCalendarObject(calendar, options) {
  var objectUrl = _url2['default'].resolve(calendar.url, options.filename);
  return webdav.createObject(objectUrl, options.data, options);
}
```
- example usage
```shell
...
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](http://doctoc.herokuapp.com/)*

- [API](#api)
- [accounts](#accounts)
  - [dav.createAccount(options)](#davcreateaccountoptions)
- [calendars](#calendars)
  - [dav.createCalendarObject(calendar, options)](#davcreatecalendarobjectcalendar-options)
  - [dav.updateCalendarObject(calendarObject, options)](#davupdatecalendarobjectcalendarobject-options)
  - [dav.deleteCalendarObject(calendarObject, options)](#davdeletecalendarobjectcalendarobject-options)
  - [dav.syncCalendar(calendar, options)](#davsynccalendarcalendar-options)
  - [dav.syncCaldavAccount(account, options)](#davsynccaldavaccountaccount-options)
- [contacts](#contacts)
  - [dav.createCard(addressBook, options)](#davcreatecardaddressbook-options)
  - [dav.updateCard(card, options)](#davupdatecardcard-options)
...
```

#### <a name="apidoc.element.dav.createCard"></a>[function <span class="apidocSignatureSpan">dav.</span>createCard (addressBook, options)](#apidoc.element.dav.createCard)
- description and source-code
```javascript
function createCard(addressBook, options) {
  var objectUrl = _url2['default'].resolve(addressBook.url, options.filename);
  return webdav.createObject(objectUrl, options.data, options);
}
```
- example usage
```shell
...
- [calendars](#calendars)
  - [dav.createCalendarObject(calendar, options)](#davcreatecalendarobjectcalendar-options)
  - [dav.updateCalendarObject(calendarObject, options)](#davupdatecalendarobjectcalendarobject-options)
  - [dav.deleteCalendarObject(calendarObject, options)](#davdeletecalendarobjectcalendarobject-options)
  - [dav.syncCalendar(calendar, options)](#davsynccalendarcalendar-options)
  - [dav.syncCaldavAccount(account, options)](#davsynccaldavaccountaccount-options)
- [contacts](#contacts)
  - [dav.createCard(addressBook, options)](#davcreatecardaddressbook-options)
  - [dav.updateCard(card, options)](#davupdatecardcard-options)
  - [dav.deleteCard(card, options)](#davdeletecardcard-options)
  - [dav.syncAddressBook(addressBook, options)](#davsyncaddressbookaddressbook-options)
  - [dav.syncCarddavAccount(account, options)](#davsynccarddavaccountaccount-options)
- [sandbox](#sandbox)
  - [dav.Sandbox()](#davsandbox)
- [transport](#transport)
...
```

#### <a name="apidoc.element.dav.createSandbox"></a>[function <span class="apidocSignatureSpan">dav.</span>createSandbox ()](#apidoc.element.dav.createSandbox)
- description and source-code
```javascript
function createSandbox() {
  return new Sandbox();
}
```
- example usage
```shell
...
'''

### sandbox

#### dav.Sandbox()

Create a request sandbox. There is also a deprecated interface
'dav.createSandbox()'. Add requests to the sandbox like so:

'''js
var sandbox = new dav.Sandbox();
// sandbox instanceof Sandbox
dav.createAccount({
username: 'Yoshi',
password: 'babybowsersoscaryomg',
...
```

#### <a name="apidoc.element.dav.debug"></a>[function <span class="apidocSignatureSpan">dav.</span>debug (topic)](#apidoc.element.dav.debug)
- description and source-code
```javascript
function debug(topic) {
  return function (message) {
    if (debug.enabled) {
      console.log("[" + topic + "] " + message);
    }
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.deleteCalendarObject"></a>[function <span class="apidocSignatureSpan">dav.</span>deleteCalendarObject (calendarObject, options)](#apidoc.element.dav.deleteCalendarObject)
- description and source-code
```javascript
function deleteCalendarObject(calendarObject, options) {
  return webdav.deleteObject(calendarObject.url, calendarObject.etag, options);
}
```
- example usage
```shell
...

- [API](#api)
- [accounts](#accounts)
  - [dav.createAccount(options)](#davcreateaccountoptions)
- [calendars](#calendars)
  - [dav.createCalendarObject(calendar, options)](#davcreatecalendarobjectcalendar-options)
  - [dav.updateCalendarObject(calendarObject, options)](#davupdatecalendarobjectcalendarobject-options)
  - [dav.deleteCalendarObject(calendarObject, options)](#davdeletecalendarobjectcalendarobject-options)
  - [dav.syncCalendar(calendar, options)](#davsynccalendarcalendar-options)
  - [dav.syncCaldavAccount(account, options)](#davsynccaldavaccountaccount-options)
- [contacts](#contacts)
  - [dav.createCard(addressBook, options)](#davcreatecardaddressbook-options)
  - [dav.updateCard(card, options)](#davupdatecardcard-options)
  - [dav.deleteCard(card, options)](#davdeletecardcard-options)
  - [dav.syncAddressBook(addressBook, options)](#davsyncaddressbookaddressbook-options)
...
```

#### <a name="apidoc.element.dav.deleteCard"></a>[function <span class="apidocSignatureSpan">dav.</span>deleteCard (card, options)](#apidoc.element.dav.deleteCard)
- description and source-code
```javascript
function deleteCard(card, options) {
  return webdav.deleteObject(card.url, card.etag, options);
}
```
- example usage
```shell
...
  - [dav.updateCalendarObject(calendarObject, options)](#davupdatecalendarobjectcalendarobject-options)
  - [dav.deleteCalendarObject(calendarObject, options)](#davdeletecalendarobjectcalendarobject-options)
  - [dav.syncCalendar(calendar, options)](#davsynccalendarcalendar-options)
  - [dav.syncCaldavAccount(account, options)](#davsynccaldavaccountaccount-options)
- [contacts](#contacts)
  - [dav.createCard(addressBook, options)](#davcreatecardaddressbook-options)
  - [dav.updateCard(card, options)](#davupdatecardcard-options)
  - [dav.deleteCard(card, options)](#davdeletecardcard-options)
  - [dav.syncAddressBook(addressBook, options)](#davsyncaddressbookaddressbook-options)
  - [dav.syncCarddavAccount(account, options)](#davsynccarddavaccountaccount-options)
- [sandbox](#sandbox)
  - [dav.Sandbox()](#davsandbox)
- [transport](#transport)
  - [dav.transport.Basic(credentials)](#davtransportbasiccredentials)
    - [dav.transport.Basic.send(request, options)](#davtransportbasicsendrequest-options)
...
```

#### <a name="apidoc.element.dav.listAddressBooks"></a>[function <span class="apidocSignatureSpan">dav.</span>listAddressBooks ()](#apidoc.element.dav.listAddressBooks)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.listCalendarObjects"></a>[function <span class="apidocSignatureSpan">dav.</span>listCalendarObjects ()](#apidoc.element.dav.listCalendarObjects)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.listCalendars"></a>[function <span class="apidocSignatureSpan">dav.</span>listCalendars ()](#apidoc.element.dav.listCalendars)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.listVCards"></a>[function <span class="apidocSignatureSpan">dav.</span>listVCards ()](#apidoc.element.dav.listVCards)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.syncAddressBook"></a>[function <span class="apidocSignatureSpan">dav.</span>syncAddressBook (addressBook, options)](#apidoc.element.dav.syncAddressBook)
- description and source-code
```javascript
function syncAddressBook(addressBook, options) {
  options.basicSync = basicSync;
  options.webdavSync = webdavSync;
  return webdav.syncCollection(addressBook, options);
}
```
- example usage
```shell
...
  - [dav.deleteCalendarObject(calendarObject, options)](#davdeletecalendarobjectcalendarobject-options)
  - [dav.syncCalendar(calendar, options)](#davsynccalendarcalendar-options)
  - [dav.syncCaldavAccount(account, options)](#davsynccaldavaccountaccount-options)
- [contacts](#contacts)
  - [dav.createCard(addressBook, options)](#davcreatecardaddressbook-options)
  - [dav.updateCard(card, options)](#davupdatecardcard-options)
  - [dav.deleteCard(card, options)](#davdeletecardcard-options)
  - [dav.syncAddressBook(addressBook, options)](#davsyncaddressbookaddressbook-options)
  - [dav.syncCarddavAccount(account, options)](#davsynccarddavaccountaccount-options)
- [sandbox](#sandbox)
  - [dav.Sandbox()](#davsandbox)
- [transport](#transport)
  - [dav.transport.Basic(credentials)](#davtransportbasiccredentials)
    - [dav.transport.Basic.send(request, options)](#davtransportbasicsendrequest-options)
  - [dav.transport.OAuth2(credentials)](#davtransportoauth2credentials)
...
```

#### <a name="apidoc.element.dav.syncCaldavAccount"></a>[function <span class="apidocSignatureSpan">dav.</span>syncCaldavAccount ()](#apidoc.element.dav.syncCaldavAccount)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
...
- [accounts](#accounts)
  - [dav.createAccount(options)](#davcreateaccountoptions)
- [calendars](#calendars)
  - [dav.createCalendarObject(calendar, options)](#davcreatecalendarobjectcalendar-options)
  - [dav.updateCalendarObject(calendarObject, options)](#davupdatecalendarobjectcalendarobject-options)
  - [dav.deleteCalendarObject(calendarObject, options)](#davdeletecalendarobjectcalendarobject-options)
  - [dav.syncCalendar(calendar, options)](#davsynccalendarcalendar-options)
  - [dav.syncCaldavAccount(account, options)](#davsynccaldavaccountaccount-options)
- [contacts](#contacts)
  - [dav.createCard(addressBook, options)](#davcreatecardaddressbook-options)
  - [dav.updateCard(card, options)](#davupdatecardcard-options)
  - [dav.deleteCard(card, options)](#davdeletecardcard-options)
  - [dav.syncAddressBook(addressBook, options)](#davsyncaddressbookaddressbook-options)
  - [dav.syncCarddavAccount(account, options)](#davsynccarddavaccountaccount-options)
- [sandbox](#sandbox)
...
```

#### <a name="apidoc.element.dav.syncCalendar"></a>[function <span class="apidocSignatureSpan">dav.</span>syncCalendar (calendar, options)](#apidoc.element.dav.syncCalendar)
- description and source-code
```javascript
function syncCalendar(calendar, options) {
  options.basicSync = basicSync;
  options.webdavSync = webdavSync;
  return webdav.syncCollection(calendar, options);
}
```
- example usage
```shell
...
- [API](#api)
- [accounts](#accounts)
  - [dav.createAccount(options)](#davcreateaccountoptions)
- [calendars](#calendars)
  - [dav.createCalendarObject(calendar, options)](#davcreatecalendarobjectcalendar-options)
  - [dav.updateCalendarObject(calendarObject, options)](#davupdatecalendarobjectcalendarobject-options)
  - [dav.deleteCalendarObject(calendarObject, options)](#davdeletecalendarobjectcalendarobject-options)
  - [dav.syncCalendar(calendar, options)](#davsynccalendarcalendar-options)
  - [dav.syncCaldavAccount(account, options)](#davsynccaldavaccountaccount-options)
- [contacts](#contacts)
  - [dav.createCard(addressBook, options)](#davcreatecardaddressbook-options)
  - [dav.updateCard(card, options)](#davupdatecardcard-options)
  - [dav.deleteCard(card, options)](#davdeletecardcard-options)
  - [dav.syncAddressBook(addressBook, options)](#davsyncaddressbookaddressbook-options)
  - [dav.syncCarddavAccount(account, options)](#davsynccarddavaccountaccount-options)
...
```

#### <a name="apidoc.element.dav.syncCarddavAccount"></a>[function <span class="apidocSignatureSpan">dav.</span>syncCarddavAccount ()](#apidoc.element.dav.syncCarddavAccount)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
...
  - [dav.syncCalendar(calendar, options)](#davsynccalendarcalendar-options)
  - [dav.syncCaldavAccount(account, options)](#davsynccaldavaccountaccount-options)
- [contacts](#contacts)
  - [dav.createCard(addressBook, options)](#davcreatecardaddressbook-options)
  - [dav.updateCard(card, options)](#davupdatecardcard-options)
  - [dav.deleteCard(card, options)](#davdeletecardcard-options)
  - [dav.syncAddressBook(addressBook, options)](#davsyncaddressbookaddressbook-options)
  - [dav.syncCarddavAccount(account, options)](#davsynccarddavaccountaccount-options)
- [sandbox](#sandbox)
  - [dav.Sandbox()](#davsandbox)
- [transport](#transport)
  - [dav.transport.Basic(credentials)](#davtransportbasiccredentials)
    - [dav.transport.Basic.send(request, options)](#davtransportbasicsendrequest-options)
  - [dav.transport.OAuth2(credentials)](#davtransportoauth2credentials)
    - [dav.transport.OAuth2.send(request, options)](#davtransportoauth2sendrequest-options)
...
```

#### <a name="apidoc.element.dav.updateCalendarObject"></a>[function <span class="apidocSignatureSpan">dav.</span>updateCalendarObject (calendarObject, options)](#apidoc.element.dav.updateCalendarObject)
- description and source-code
```javascript
function updateCalendarObject(calendarObject, options) {
  return webdav.updateObject(calendarObject.url, calendarObject.calendarData, calendarObject.etag, options);
}
```
- example usage
```shell
...
**Table of Contents**  *generated with [DocToc](http://doctoc.herokuapp.com/)*

- [API](#api)
- [accounts](#accounts)
  - [dav.createAccount(options)](#davcreateaccountoptions)
- [calendars](#calendars)
  - [dav.createCalendarObject(calendar, options)](#davcreatecalendarobjectcalendar-options)
  - [dav.updateCalendarObject(calendarObject, options)](#davupdatecalendarobjectcalendarobject-options)
  - [dav.deleteCalendarObject(calendarObject, options)](#davdeletecalendarobjectcalendarobject-options)
  - [dav.syncCalendar(calendar, options)](#davsynccalendarcalendar-options)
  - [dav.syncCaldavAccount(account, options)](#davsynccaldavaccountaccount-options)
- [contacts](#contacts)
  - [dav.createCard(addressBook, options)](#davcreatecardaddressbook-options)
  - [dav.updateCard(card, options)](#davupdatecardcard-options)
  - [dav.deleteCard(card, options)](#davdeletecardcard-options)
...
```

#### <a name="apidoc.element.dav.updateCard"></a>[function <span class="apidocSignatureSpan">dav.</span>updateCard (card, options)](#apidoc.element.dav.updateCard)
- description and source-code
```javascript
function updateCard(card, options) {
  return webdav.updateObject(card.url, card.addressData, card.etag, options);
}
```
- example usage
```shell
...
  - [dav.createCalendarObject(calendar, options)](#davcreatecalendarobjectcalendar-options)
  - [dav.updateCalendarObject(calendarObject, options)](#davupdatecalendarobjectcalendarobject-options)
  - [dav.deleteCalendarObject(calendarObject, options)](#davdeletecalendarobjectcalendarobject-options)
  - [dav.syncCalendar(calendar, options)](#davsynccalendarcalendar-options)
  - [dav.syncCaldavAccount(account, options)](#davsynccaldavaccountaccount-options)
- [contacts](#contacts)
  - [dav.createCard(addressBook, options)](#davcreatecardaddressbook-options)
  - [dav.updateCard(card, options)](#davupdatecardcard-options)
  - [dav.deleteCard(card, options)](#davdeletecardcard-options)
  - [dav.syncAddressBook(addressBook, options)](#davsyncaddressbookaddressbook-options)
  - [dav.syncCarddavAccount(account, options)](#davsynccarddavaccountaccount-options)
- [sandbox](#sandbox)
  - [dav.Sandbox()](#davsandbox)
- [transport](#transport)
  - [dav.transport.Basic(credentials)](#davtransportbasiccredentials)
...
```



# <a name="apidoc.module.dav.createAccount"></a>[module dav.createAccount](#apidoc.module.dav.createAccount)

#### <a name="apidoc.element.dav.createAccount.createAccount"></a>[function <span class="apidocSignatureSpan">dav.</span>createAccount ()](#apidoc.element.dav.createAccount.createAccount)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
...

<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](http://doctoc.herokuapp.com/)*

- [API](#api)
- [accounts](#accounts)
  - [dav.createAccount(options)](#davcreateaccountoptions)
- [calendars](#calendars)
  - [dav.createCalendarObject(calendar, options)](#davcreatecalendarobjectcalendar-options)
  - [dav.updateCalendarObject(calendarObject, options)](#davupdatecalendarobjectcalendarobject-options)
  - [dav.deleteCalendarObject(calendarObject, options)](#davdeletecalendarobjectcalendarobject-options)
  - [dav.syncCalendar(calendar, options)](#davsynccalendarcalendar-options)
  - [dav.syncCaldavAccount(account, options)](#davsynccaldavaccountaccount-options)
- [contacts](#contacts)
...
```

#### <a name="apidoc.element.dav.createAccount.__generatorFunction__"></a>[function <span class="apidocSignatureSpan">dav.createAccount.</span>__generatorFunction__ (options)](#apidoc.element.dav.createAccount.__generatorFunction__)
- description and source-code
```javascript
function callee$0$0(options) {
  var account, key, loadCollections, loadObjects, collections;
  return regeneratorRuntime.wrap(function callee$0$0$(context$1$0) {
    while (1) switch (context$1$0.prev = context$1$0.next) {
      case 0:
        options = Object.assign({}, defaults, options);
        if (typeof options.loadObjects !== 'boolean') {
          options.loadObjects = options.loadCollections;
        }

        account = new _model.Account({
          server: options.server,
          credentials: options.xhr.credentials
        });
        context$1$0.next = 5;
        return serviceDiscovery(account, options);

      case 5:
        account.rootUrl = context$1$0.sent;
        context$1$0.next = 8;
        return principalUrl(account, options);

      case 8:
        account.principalUrl = context$1$0.sent;
        context$1$0.next = 11;
        return homeUrl(account, options);

      case 11:
        account.homeUrl = context$1$0.sent;

        if (options.loadCollections) {
          context$1$0.next = 14;
          break;
        }

        return context$1$0.abrupt('return', account);

      case 14:
        key = undefined, loadCollections = undefined, loadObjects = undefined;

        if (options.accountType === 'caldav') {
          key = 'calendars';
          loadCollections = _calendars.listCalendars;
          loadObjects = _calendars.listCalendarObjects;
        } else if (options.accountType === 'carddav') {
          key = 'addressBooks';
          loadCollections = _contacts.listAddressBooks;
          loadObjects = _contacts.listVCards;
        }

        context$1$0.next = 18;
        return loadCollections(account, options);

      case 18:
        collections = context$1$0.sent;

        account[key] = collections;

        if (options.loadObjects) {
          context$1$0.next = 22;
          break;
        }

        return context$1$0.abrupt('return', account);

      case 22:
        context$1$0.next = 24;
        return collections.map(_co2['default'].wrap(regeneratorRuntime.mark(function callee$1$0(collection) {
          return regeneratorRuntime.wrap(function callee$1$0$(context$2$0) {
            while (1) switch (context$2$0.prev = context$2$0.next) {
              case 0:
                context$2$0.prev = 0;
                context$2$0.next = 3;
                return loadObjects(collection, options);

              case 3:
                collection.objects = context$2$0.sent;
                context$2$0.next = 9;
                break;

              case 6:
                context$2$0.prev = 6;
                context$2$0.t0 = context$2$0['catch'](0);

                collection.error = context$2$0.t0;

              case 9:
              case 'end':
                return context$2$0.stop();
            }
          }, callee$1$0, this, [[0, 6]]);
        })));

      case 24:

        account[key] = account[key].filter(function (collection) {
          return !collection.error;
        });

        return context$1$0.abrupt('return', account);

      case 26:
      case 'end':
        return context$1$0.stop();
    }
  }, callee$0$0, this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.dav.listAddressBooks"></a>[module dav.listAddressBooks](#apidoc.module.dav.listAddressBooks)

#### <a name="apidoc.element.dav.listAddressBooks.listAddressBooks"></a>[function <span class="apidocSignatureSpan">dav.</span>listAddressBooks ()](#apidoc.element.dav.listAddressBooks.listAddressBooks)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.listAddressBooks.__generatorFunction__"></a>[function <span class="apidocSignatureSpan">dav.listAddressBooks.</span>__generatorFunction__ (account, options)](#apidoc.element.dav.listAddressBooks.__generatorFunction__)
- description and source-code
```javascript
function callee$0$0(account, options) {
  var req, responses, addressBooks;
  return regeneratorRuntime.wrap(function callee$0$0$(context$1$0) {
    while (1) switch (context$1$0.prev = context$1$0.next) {
      case 0:
        debug('Fetch address books from home url ' + account.homeUrl);
        req = request.propfind({
          props: [{ name: 'displayname', namespace: ns.DAV }, { name: 'getctag', namespace: ns.CALENDAR_SERVER }, { name: 'resourcetype
', namespace: ns.DAV }, { name: 'sync-token', namespace: ns.DAV }],
          depth: 1
        });
        context$1$0.next = 4;
        return options.xhr.send(req, account.homeUrl, {
          sandbox: options.sandbox
        });

      case 4:
        responses = context$1$0.sent;
        addressBooks = responses.filter(function (res) {
          return typeof res.props.displayname === 'string';
        }).map(function (res) {
          debug('Found address book named ' + res.props.displayname + ',\n             props: ' + JSON.stringify(res.props));
          return new _model.AddressBook({
            data: res,
            account: account,
            url: _url2['default'].resolve(account.rootUrl, res.href),
            ctag: res.props.getctag,
            displayName: res.props.displayname,
            resourcetype: res.props.resourcetype,
            syncToken: res.props.syncToken
          });
        });
        context$1$0.next = 8;
        return addressBooks.map(_co2['default'].wrap(regeneratorRuntime.mark(function callee$1$0(addressBook) {
          return regeneratorRuntime.wrap(function callee$1$0$(context$2$0) {
            while (1) switch (context$2$0.prev = context$2$0.next) {
              case 0:
                context$2$0.next = 2;
                return webdav.supportedReportSet(addressBook, options);

              case 2:
                addressBook.reports = context$2$0.sent;

              case 3:
              case 'end':
                return context$2$0.stop();
            }
          }, callee$1$0, this);
        })));

      case 8:
        return context$1$0.abrupt('return', addressBooks);

      case 9:
      case 'end':
        return context$1$0.stop();
    }
  }, callee$0$0, this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.dav.listCalendarObjects"></a>[module dav.listCalendarObjects](#apidoc.module.dav.listCalendarObjects)

#### <a name="apidoc.element.dav.listCalendarObjects.listCalendarObjects"></a>[function <span class="apidocSignatureSpan">dav.</span>listCalendarObjects ()](#apidoc.element.dav.listCalendarObjects.listCalendarObjects)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.listCalendarObjects.__generatorFunction__"></a>[function <span class="apidocSignatureSpan">dav.listCalendarObjects.</span>__generatorFunction__ (calendar, options)](#apidoc.element.dav.listCalendarObjects.__generatorFunction__)
- description and source-code
```javascript
function callee$0$0(calendar, options) {
  var filters, req, responses;
  return regeneratorRuntime.wrap(function callee$0$0$(context$1$0) {
    while (1) switch (context$1$0.prev = context$1$0.next) {
      case 0:
        debug('Doing REPORT on calendar ' + calendar.url + ' which belongs to\n         ' + calendar.account.credentials.username
);

        filters = options.filters || [{
          type: 'comp-filter',
          attrs: { name: 'VCALENDAR' },
          children: [{
            type: 'comp-filter',
            attrs: { name: 'VEVENT' }
          }]
        }];
        req = request.calendarQuery({
          depth: 1,
          props: [{ name: 'getetag', namespace: ns.DAV }, { name: 'calendar-data', namespace: ns.CALDAV }],
          filters: filters
        });
        context$1$0.next = 5;
        return options.xhr.send(req, calendar.url, {
          sandbox: options.sandbox
        });

      case 5:
        responses = context$1$0.sent;
        return context$1$0.abrupt('return', responses.map(function (res) {
          debug('Found calendar object with url ' + res.href);
          return new _model.CalendarObject({
            data: res,
            calendar: calendar,
            url: _url2['default'].resolve(calendar.account.rootUrl, res.href),
            etag: res.props.getetag,
            calendarData: res.props.calendarData
          });
        }));

      case 7:
      case 'end':
        return context$1$0.stop();
    }
  }, callee$0$0, this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.dav.listCalendars"></a>[module dav.listCalendars](#apidoc.module.dav.listCalendars)

#### <a name="apidoc.element.dav.listCalendars.listCalendars"></a>[function <span class="apidocSignatureSpan">dav.</span>listCalendars ()](#apidoc.element.dav.listCalendars.listCalendars)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.listCalendars.__generatorFunction__"></a>[function <span class="apidocSignatureSpan">dav.listCalendars.</span>__generatorFunction__ (account, options)](#apidoc.element.dav.listCalendars.__generatorFunction__)
- description and source-code
```javascript
function callee$0$0(account, options) {
  var req, responses, cals;
  return regeneratorRuntime.wrap(function callee$0$0$(context$1$0) {
    while (1) switch (context$1$0.prev = context$1$0.next) {
      case 0:
        debug('Fetch calendars from home url ' + account.homeUrl);
        req = request.propfind({
          props: [{ name: 'calendar-description', namespace: ns.CALDAV }, { name: 'calendar-timezone', namespace: ns.CALDAV }, {
name: 'displayname', namespace: ns.DAV }, { name: 'getctag', namespace: ns.CALENDAR_SERVER }, { name: 'resourcetype', namespace:
ns.DAV }, { name: 'supported-calendar-component-set', namespace: ns.CALDAV }, { name: 'sync-token', namespace: ns.DAV }],
          depth: 1
        });
        context$1$0.next = 4;
        return options.xhr.send(req, account.homeUrl, {
          sandbox: options.sandbox
        });

      case 4:
        responses = context$1$0.sent;

        debug('Found ' + responses.length + ' calendars.');
        cals = responses.filter(function (res) {
          // We only want the calendar if it contains iCalendar objects.
          var components = res.props.supportedCalendarComponentSet || [];
          return components.reduce(function (hasObjs, component) {
            return hasObjs || ICAL_OBJS.has(component);
          }, false);
        }).map(function (res) {
          debug('Found calendar ' + res.props.displayname + ',\n             props: ' + JSON.stringify(res.props));
          return new _model.Calendar({
            data: res,
            account: account,
            description: res.props.calendarDescription,
            timezone: res.props.calendarTimezone,
            url: _url2['default'].resolve(account.rootUrl, res.href),
            ctag: res.props.getctag,
            displayName: res.props.displayname,
            components: res.props.supportedCalendarComponentSet,
            resourcetype: res.props.resourcetype,
            syncToken: res.props.syncToken
          });
        });
        context$1$0.next = 9;
        return cals.map(_co2['default'].wrap(regeneratorRuntime.mark(function callee$1$0(cal) {
          return regeneratorRuntime.wrap(function callee$1$0$(context$2$0) {
            while (1) switch (context$2$0.prev = context$2$0.next) {
              case 0:
                context$2$0.next = 2;
                return webdav.supportedReportSet(cal, options);

              case 2:
                cal.reports = context$2$0.sent;

              case 3:
              case 'end':
                return context$2$0.stop();
            }
          }, callee$1$0, this);
        })));

      case 9:
        return context$1$0.abrupt('return', cals);

      case 10:
      case 'end':
        return context$1$0.stop();
    }
  }, callee$0$0, this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.dav.listVCards"></a>[module dav.listVCards](#apidoc.module.dav.listVCards)

#### <a name="apidoc.element.dav.listVCards.listVCards"></a>[function <span class="apidocSignatureSpan">dav.</span>listVCards ()](#apidoc.element.dav.listVCards.listVCards)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.listVCards.__generatorFunction__"></a>[function <span class="apidocSignatureSpan">dav.listVCards.</span>__generatorFunction__ (addressBook, options)](#apidoc.element.dav.listVCards.__generatorFunction__)
- description and source-code
```javascript
function callee$0$0(addressBook, options) {
  var req, responses;
  return regeneratorRuntime.wrap(function callee$0$0$(context$1$0) {
    while (1) switch (context$1$0.prev = context$1$0.next) {
      case 0:
        debug('Doing REPORT on address book ' + addressBook.url + ' which belongs to\n        ' + addressBook.account.credentials
.username);

        req = request.addressBookQuery({
          depth: 1,
          props: [{ name: 'getetag', namespace: ns.DAV }, { name: 'address-data', namespace: ns.CARDDAV }]
        });
        context$1$0.next = 4;
        return options.xhr.send(req, addressBook.url, {
          sandbox: options.sandbox
        });

      case 4:
        responses = context$1$0.sent;
        return context$1$0.abrupt('return', responses.map(function (res) {
          debug('Found vcard with url ' + res.href);
          return new _model.VCard({
            data: res,
            addressBook: addressBook,
            url: _url2['default'].resolve(addressBook.account.rootUrl, res.href),
            etag: res.props.getetag,
            addressData: res.props.addressData
          });
        }));

      case 6:
      case 'end':
        return context$1$0.stop();
    }
  }, callee$0$0, this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.dav.request"></a>[module dav.request](#apidoc.module.dav.request)

#### <a name="apidoc.element.dav.request.Request"></a>[function <span class="apidocSignatureSpan">dav.request.</span>Request ()](#apidoc.element.dav.request.Request)
- description and source-code
```javascript
function Request() {
  var options = arguments.length <= 0 || arguments[0] === undefined ? {} : arguments[0];

  _classCallCheck(this, Request);

  Object.assign(this, {
    method: null,
    requestData: null,
    transformRequest: null,
    transformResponse: null,
    onerror: null
  }, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.request.addressBookQuery"></a>[function <span class="apidocSignatureSpan">dav.request.</span>addressBookQuery (options)](#apidoc.element.dav.request.addressBookQuery)
- description and source-code
```javascript
function addressBookQuery(options) {
  return collectionQuery(template.addressBookQuery({ props: options.props || [] }), { depth: options.depth });
}
```
- example usage
```shell
...
  - [dav.Sandbox()](#davsandbox)
- [transport](#transport)
  - [dav.transport.Basic(credentials)](#davtransportbasiccredentials)
    - [dav.transport.Basic.send(request, options)](#davtransportbasicsendrequest-options)
  - [dav.transport.OAuth2(credentials)](#davtransportoauth2credentials)
    - [dav.transport.OAuth2.send(request, options)](#davtransportoauth2sendrequest-options)
- [request](#request)
  - [dav.request.addressBookQuery(options)](#davrequestaddressbookqueryoptions)
  - [dav.request.basic(options)](#davrequestbasicoptions)
  - [dav.request.calendarQuery(options)](#davrequestcalendarqueryoptions)
  - [dav.request.propfind(options)](#davrequestpropfindoptions)
  - [dav.request.syncCollection(options)](#davrequestsynccollectionoptions)
- [Client](#client)
  - [dav.Client(xhr, options)](#davclientxhr-options)
    - [dav.Client.send(req, options)](#davclientsendreq-options)
...
```

#### <a name="apidoc.element.dav.request.basic"></a>[function <span class="apidocSignatureSpan">dav.request.</span>basic (options)](#apidoc.element.dav.request.basic)
- description and source-code
```javascript
function basic(options) {
  function transformRequest(xhr) {
    setRequestHeaders(xhr, options);
  }

  return new Request({
    method: options.method,
    requestData: options.data,
    transformRequest: transformRequest
  });
}
```
- example usage
```shell
...
- [transport](#transport)
  - [dav.transport.Basic(credentials)](#davtransportbasiccredentials)
    - [dav.transport.Basic.send(request, options)](#davtransportbasicsendrequest-options)
  - [dav.transport.OAuth2(credentials)](#davtransportoauth2credentials)
    - [dav.transport.OAuth2.send(request, options)](#davtransportoauth2sendrequest-options)
- [request](#request)
  - [dav.request.addressBookQuery(options)](#davrequestaddressbookqueryoptions)
  - [dav.request.basic(options)](#davrequestbasicoptions)
  - [dav.request.calendarQuery(options)](#davrequestcalendarqueryoptions)
  - [dav.request.propfind(options)](#davrequestpropfindoptions)
  - [dav.request.syncCollection(options)](#davrequestsynccollectionoptions)
- [Client](#client)
  - [dav.Client(xhr, options)](#davclientxhr-options)
    - [dav.Client.send(req, options)](#davclientsendreq-options)
- [etc](#etc)
...
```

#### <a name="apidoc.element.dav.request.calendarQuery"></a>[function <span class="apidocSignatureSpan">dav.request.</span>calendarQuery (options)](#apidoc.element.dav.request.calendarQuery)
- description and source-code
```javascript
function calendarQuery(options) {
  return collectionQuery(template.calendarQuery({
    props: options.props || [],
    filters: options.filters || [],
    timezone: options.timezone
  }), {
    depth: options.depth
  });
}
```
- example usage
```shell
...
  - [dav.transport.Basic(credentials)](#davtransportbasiccredentials)
    - [dav.transport.Basic.send(request, options)](#davtransportbasicsendrequest-options)
  - [dav.transport.OAuth2(credentials)](#davtransportoauth2credentials)
    - [dav.transport.OAuth2.send(request, options)](#davtransportoauth2sendrequest-options)
- [request](#request)
  - [dav.request.addressBookQuery(options)](#davrequestaddressbookqueryoptions)
  - [dav.request.basic(options)](#davrequestbasicoptions)
  - [dav.request.calendarQuery(options)](#davrequestcalendarqueryoptions)
  - [dav.request.propfind(options)](#davrequestpropfindoptions)
  - [dav.request.syncCollection(options)](#davrequestsynccollectionoptions)
- [Client](#client)
  - [dav.Client(xhr, options)](#davclientxhr-options)
    - [dav.Client.send(req, options)](#davclientsendreq-options)
- [etc](#etc)
  - [dav.ns](#davns)
...
```

#### <a name="apidoc.element.dav.request.collectionQuery"></a>[function <span class="apidocSignatureSpan">dav.request.</span>collectionQuery (requestData, options)](#apidoc.element.dav.request.collectionQuery)
- description and source-code
```javascript
function collectionQuery(requestData, options) {
  function transformRequest(xhr) {
    setRequestHeaders(xhr, options);
  }

  function transformResponse(xhr) {
    return (0, _parser.multistatus)(xhr.responseText).response.map(function (res) {
      return { href: res.href, props: getProps(res.propstat) };
    });
  }

  return new Request({
    method: 'REPORT',
    requestData: requestData,
    transformRequest: transformRequest,
    transformResponse: transformResponse
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.request.getProps"></a>[function <span class="apidocSignatureSpan">dav.request.</span>getProps (propstats)](#apidoc.element.dav.request.getProps)
- description and source-code
```javascript
function getProps(propstats) {
  return mergeProps(propstats.map(getProp).filter(function (prop) {
    return prop && typeof prop === 'object';
  }));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.request.mergeProps"></a>[function <span class="apidocSignatureSpan">dav.request.</span>mergeProps (props)](#apidoc.element.dav.request.mergeProps)
- description and source-code
```javascript
function mergeProps(props) {
  return props.reduce(function (a, b) {
    return Object.assign(a, b);
  }, {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.request.propfind"></a>[function <span class="apidocSignatureSpan">dav.request.</span>propfind (options)](#apidoc.element.dav.request.propfind)
- description and source-code
```javascript
function propfind(options) {
  var requestData = template.propfind({ props: options.props });

  function transformRequest(xhr) {
    setRequestHeaders(xhr, options);
  }

  function transformResponse(xhr) {
    var responses = (0, _parser.multistatus)(xhr.responseText).response.map(function (res) {
      return { href: res.href, props: getProps(res.propstat) };
    });

    if (!options.mergeResponses) {
      return responses;
    }

    // Merge the props.
    var merged = mergeProps(responses.map(function (res) {
      return res.props;
    }));
    var hrefs = responses.map(function (res) {
      return res.href;
    });
    return { props: merged, hrefs: hrefs };
  }

  return new Request({
    method: 'PROPFIND',
    requestData: requestData,
    transformRequest: transformRequest,
    transformResponse: transformResponse
  });
}
```
- example usage
```shell
...
    - [dav.transport.Basic.send(request, options)](#davtransportbasicsendrequest-options)
  - [dav.transport.OAuth2(credentials)](#davtransportoauth2credentials)
    - [dav.transport.OAuth2.send(request, options)](#davtransportoauth2sendrequest-options)
- [request](#request)
  - [dav.request.addressBookQuery(options)](#davrequestaddressbookqueryoptions)
  - [dav.request.basic(options)](#davrequestbasicoptions)
  - [dav.request.calendarQuery(options)](#davrequestcalendarqueryoptions)
  - [dav.request.propfind(options)](#davrequestpropfindoptions)
  - [dav.request.syncCollection(options)](#davrequestsynccollectionoptions)
- [Client](#client)
  - [dav.Client(xhr, options)](#davclientxhr-options)
    - [dav.Client.send(req, options)](#davclientsendreq-options)
- [etc](#etc)
  - [dav.ns](#davns)
- [Example Usage](#example-usage)
...
```

#### <a name="apidoc.element.dav.request.setRequestHeaders"></a>[function <span class="apidocSignatureSpan">dav.request.</span>setRequestHeaders (request, options)](#apidoc.element.dav.request.setRequestHeaders)
- description and source-code
```javascript
function setRequestHeaders(request, options) {
  request.setRequestHeader('Content-Type', 'application/xml;charset=utf-8');

  if ('depth' in options) {
    request.setRequestHeader('Depth', options.depth);
  }

  if ('etag' in options) {
    request.setRequestHeader('If-Match', options.etag);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.dav.request.syncCollection"></a>[function <span class="apidocSignatureSpan">dav.request.</span>syncCollection (options)](#apidoc.element.dav.request.syncCollection)
- description and source-code
```javascript
function syncCollection(options) {
  var requestData = template.syncCollection({
    props: options.props,
    syncLevel: options.syncLevel,
    syncToken: options.syncToken
  });

  function transformRequest(xhr) {
    setRequestHeaders(xhr, options);
  }

  function transformResponse(xhr) {
    var object = (0, _parser.multistatus)(xhr.responseText);
    var responses = object.response.map(function (res) {
      return { href: res.href, props: getProps(res.propstat) };
    });

    return { responses: responses, syncToken: object.syncToken };
  }

  return new Request({
    method: 'REPORT',
    requestData: requestData,
    transformRequest: transformRequest,
    transformResponse: transformResponse
  });
}
```
- example usage
```shell
...
  - [dav.transport.OAuth2(credentials)](#davtransportoauth2credentials)
    - [dav.transport.OAuth2.send(request, options)](#davtransportoauth2sendrequest-options)
- [request](#request)
  - [dav.request.addressBookQuery(options)](#davrequestaddressbookqueryoptions)
  - [dav.request.basic(options)](#davrequestbasicoptions)
  - [dav.request.calendarQuery(options)](#davrequestcalendarqueryoptions)
  - [dav.request.propfind(options)](#davrequestpropfindoptions)
  - [dav.request.syncCollection(options)](#davrequestsynccollectionoptions)
- [Client](#client)
  - [dav.Client(xhr, options)](#davclientxhr-options)
    - [dav.Client.send(req, options)](#davclientsendreq-options)
- [etc](#etc)
  - [dav.ns](#davns)
- [Example Usage](#example-usage)
  - [Using the lower-level webdav request api](#using-the-lower-level-webdav-request-api)
...
```



# <a name="apidoc.module.dav.syncCaldavAccount"></a>[module dav.syncCaldavAccount](#apidoc.module.dav.syncCaldavAccount)

#### <a name="apidoc.element.dav.syncCaldavAccount.syncCaldavAccount"></a>[function <span class="apidocSignatureSpan">dav.</span>syncCaldavAccount ()](#apidoc.element.dav.syncCaldavAccount.syncCaldavAccount)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
...
- [accounts](#accounts)
  - [dav.createAccount(options)](#davcreateaccountoptions)
- [calendars](#calendars)
  - [dav.createCalendarObject(calendar, options)](#davcreatecalendarobjectcalendar-options)
  - [dav.updateCalendarObject(calendarObject, options)](#davupdatecalendarobjectcalendarobject-options)
  - [dav.deleteCalendarObject(calendarObject, options)](#davdeletecalendarobjectcalendarobject-options)
  - [dav.syncCalendar(calendar, options)](#davsynccalendarcalendar-options)
  - [dav.syncCaldavAccount(account, options)](#davsynccaldavaccountaccount-options)
- [contacts](#contacts)
  - [dav.createCard(addressBook, options)](#davcreatecardaddressbook-options)
  - [dav.updateCard(card, options)](#davupdatecardcard-options)
  - [dav.deleteCard(card, options)](#davdeletecardcard-options)
  - [dav.syncAddressBook(addressBook, options)](#davsyncaddressbookaddressbook-options)
  - [dav.syncCarddavAccount(account, options)](#davsynccarddavaccountaccount-options)
- [sandbox](#sandbox)
...
```

#### <a name="apidoc.element.dav.syncCaldavAccount.__generatorFunction__"></a>[function <span class="apidocSignatureSpan">dav.syncCaldavAccount.</span>__generatorFunction__ (account)](#apidoc.element.dav.syncCaldavAccount.__generatorFunction__)
- description and source-code
```javascript
function callee$0$0(account) {
  var options = arguments.length <= 1 || arguments[1] === undefined ? {} : arguments[1];
  var cals;
  return regeneratorRuntime.wrap(function callee$0$0$(context$1$0) {
    while (1) switch (context$1$0.prev = context$1$0.next) {
      case 0:
        options.loadObjects = false;
        if (!account.calendars) account.calendars = [];

        context$1$0.next = 4;
        return listCalendars(account, options);

      case 4:
        cals = context$1$0.sent;

        cals.filter(function (cal) {
          // Filter the calendars not previously seen.
          return account.calendars.every(function (prev) {
            return !(0, _fuzzy_url_equals2['default'])(prev.url, cal.url);
          });
        }).forEach(function (cal) {
          // Add them to the account's calendar list.
          account.calendars.push(cal);
        });

        options.loadObjects = true;
        context$1$0.next = 9;
        return account.calendars.map(_co2['default'].wrap(regeneratorRuntime.mark(function callee$1$0(cal, index) {
          return regeneratorRuntime.wrap(function callee$1$0$(context$2$0) {
            while (1) switch (context$2$0.prev = context$2$0.next) {
              case 0:
                context$2$0.prev = 0;
                context$2$0.next = 3;
                return syncCalendar(cal, options);

              case 3:
                context$2$0.next = 9;
                break;

              case 5:
                context$2$0.prev = 5;
                context$2$0.t0 = context$2$0['catch'](0);

                debug('Sync calendar ' + cal.displayName + ' failed with ' + context$2$0.t0);
                account.calendars.splice(index, 1);

              case 9:
              case 'end':
                return context$2$0.stop();
            }
          }, callee$1$0, this, [[0, 5]]);
        })));

      case 9:
        return context$1$0.abrupt('return', account);

      case 10:
      case 'end':
        return context$1$0.stop();
    }
  }, callee$0$0, this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.dav.syncCarddavAccount"></a>[module dav.syncCarddavAccount](#apidoc.module.dav.syncCarddavAccount)

#### <a name="apidoc.element.dav.syncCarddavAccount.syncCarddavAccount"></a>[function <span class="apidocSignatureSpan">dav.</span>syncCarddavAccount ()](#apidoc.element.dav.syncCarddavAccount.syncCarddavAccount)
- description and source-code
```javascript
function createPromise() {
  return co.call(this, fn.apply(this, arguments));
}
```
- example usage
```shell
...
  - [dav.syncCalendar(calendar, options)](#davsynccalendarcalendar-options)
  - [dav.syncCaldavAccount(account, options)](#davsynccaldavaccountaccount-options)
- [contacts](#contacts)
  - [dav.createCard(addressBook, options)](#davcreatecardaddressbook-options)
  - [dav.updateCard(card, options)](#davupdatecardcard-options)
  - [dav.deleteCard(card, options)](#davdeletecardcard-options)
  - [dav.syncAddressBook(addressBook, options)](#davsyncaddressbookaddressbook-options)
  - [dav.syncCarddavAccount(account, options)](#davsynccarddavaccountaccount-options)
- [sandbox](#sandbox)
  - [dav.Sandbox()](#davsandbox)
- [transport](#transport)
  - [dav.transport.Basic(credentials)](#davtransportbasiccredentials)
    - [dav.transport.Basic.send(request, options)](#davtransportbasicsendrequest-options)
  - [dav.transport.OAuth2(credentials)](#davtransportoauth2credentials)
    - [dav.transport.OAuth2.send(request, options)](#davtransportoauth2sendrequest-options)
...
```

#### <a name="apidoc.element.dav.syncCarddavAccount.__generatorFunction__"></a>[function <span class="apidocSignatureSpan">dav.syncCarddavAccount.</span>__generatorFunction__ (account)](#apidoc.element.dav.syncCarddavAccount.__generatorFunction__)
- description and source-code
```javascript
function callee$0$0(account) {
  var options = arguments.length <= 1 || arguments[1] === undefined ? {} : arguments[1];
  var addressBooks;
  return regeneratorRuntime.wrap(function callee$0$0$(context$1$0) {
    while (1) switch (context$1$0.prev = context$1$0.next) {
      case 0:
        options.loadObjects = false;

        if (!account.addressBooks) {
          account.addressBooks = [];
        }

        context$1$0.next = 4;
        return listAddressBooks(account, options);

      case 4:
        addressBooks = context$1$0.sent;

        addressBooks.filter(function (addressBook) {
          // Filter the address books not previously seen.
          return account.addressBooks.every(function (prev) {
            return !(0, _fuzzy_url_equals2['default'])(prev.url, addressBook.url);
          });
        }).forEach(function (addressBook) {
          return account.addressBooks.push(addressBook);
        });

        options.loadObjects = true;
        context$1$0.next = 9;
        return account.addressBooks.map(_co2['default'].wrap(regeneratorRuntime.mark(function callee$1$0(addressBook, index) {
          return regeneratorRuntime.wrap(function callee$1$0$(context$2$0) {
            while (1) switch (context$2$0.prev = context$2$0.next) {
              case 0:
                context$2$0.prev = 0;
                context$2$0.next = 3;
                return syncAddressBook(addressBook, options);

              case 3:
                context$2$0.next = 9;
                break;

              case 5:
                context$2$0.prev = 5;
                context$2$0.t0 = context$2$0['catch'](0);

                debug('Syncing ' + addressBook.displayName + ' failed with ' + context$2$0.t0);
                account.addressBooks.splice(index, 1);

              case 9:
              case 'end':
                return context$2$0.stop();
            }
          }, callee$1$0, this, [[0, 5]]);
        })));

      case 9:
        return context$1$0.abrupt('return', account);

      case 10:
      case 'end':
        return context$1$0.stop();
    }
  }, callee$0$0, this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.dav.transport"></a>[module dav.transport](#apidoc.module.dav.transport)

#### <a name="apidoc.element.dav.transport.Basic"></a>[function <span class="apidocSignatureSpan">dav.transport.</span>Basic (credentials)](#apidoc.element.dav.transport.Basic)
- description and source-code
```javascript
function Basic(credentials) {
  _classCallCheck(this, Basic);

  _get(Object.getPrototypeOf(Basic.prototype), 'constructor', this).call(this, credentials);
}
```
- example usage
```shell
...
  - [dav.updateCard(card, options)](#davupdatecardcard-options)
  - [dav.deleteCard(card, options)](#davdeletecardcard-options)
  - [dav.syncAddressBook(addressBook, options)](#davsyncaddressbookaddressbook-options)
  - [dav.syncCarddavAccount(account, options)](#davsynccarddavaccountaccount-options)
- [sandbox](#sandbox)
  - [dav.Sandbox()](#davsandbox)
- [transport](#transport)
  - [dav.transport.Basic(credentials)](#davtransportbasiccredentials)
    - [dav.transport.Basic.send(request, options)](#davtransportbasicsendrequest-options)
  - [dav.transport.OAuth2(credentials)](#davtransportoauth2credentials)
    - [dav.transport.OAuth2.send(request, options)](#davtransportoauth2sendrequest-options)
- [request](#request)
  - [dav.request.addressBookQuery(options)](#davrequestaddressbookqueryoptions)
  - [dav.request.basic(options)](#davrequestbasicoptions)
  - [dav.request.calendarQuery(options)](#davrequestcalendarqueryoptions)
...
```

#### <a name="apidoc.element.dav.transport.OAuth2"></a>[function <span class="apidocSignatureSpan">dav.transport.</span>OAuth2 (credentials)](#apidoc.element.dav.transport.OAuth2)
- description and source-code
```javascript
function OAuth2(credentials) {
  _classCallCheck(this, OAuth2);

  _get(Object.getPrototypeOf(OAuth2.prototype), 'constructor', this).call(this, credentials);
}
```
- example usage
```shell
...
  - [dav.syncAddressBook(addressBook, options)](#davsyncaddressbookaddressbook-options)
  - [dav.syncCarddavAccount(account, options)](#davsynccarddavaccountaccount-options)
- [sandbox](#sandbox)
  - [dav.Sandbox()](#davsandbox)
- [transport](#transport)
  - [dav.transport.Basic(credentials)](#davtransportbasiccredentials)
    - [dav.transport.Basic.send(request, options)](#davtransportbasicsendrequest-options)
  - [dav.transport.OAuth2(credentials)](#davtransportoauth2credentials)
    - [dav.transport.OAuth2.send(request, options)](#davtransportoauth2sendrequest-options)
- [request](#request)
  - [dav.request.addressBookQuery(options)](#davrequestaddressbookqueryoptions)
  - [dav.request.basic(options)](#davrequestbasicoptions)
  - [dav.request.calendarQuery(options)](#davrequestcalendarqueryoptions)
  - [dav.request.propfind(options)](#davrequestpropfindoptions)
  - [dav.request.syncCollection(options)](#davrequestsynccollectionoptions)
...
```

#### <a name="apidoc.element.dav.transport.Transport"></a>[function <span class="apidocSignatureSpan">dav.transport.</span>Transport (credentials)](#apidoc.element.dav.transport.Transport)
- description and source-code
```javascript
function Transport(credentials) {
  _classCallCheck(this, Transport);

  this.credentials = credentials || null;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
