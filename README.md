# api documentation for  [node-mysql (v0.4.2)](https://github.com/redblaze/node-mysql)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-mysql.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-mysql) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-mysql.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-mysql)
#### A wrapper of node.js mysql package to make it a bit easier to use.

[![NPM](https://nodei.co/npm/node-mysql.png?downloads=true)](https://www.npmjs.com/package/node-mysql)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-mysql/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-node-mysql_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-mysql/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-mysql/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-mysql/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Chiyan Chen"
    },
    "bugs": {
        "url": "https://github.com/redblaze/node-mysql/issues"
    },
    "dependencies": {
        "better-js-class": "*",
        "cps": "*",
        "mysql": "*",
        "underscore": "*"
    },
    "description": "A wrapper of node.js mysql package to make it a bit easier to use.",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "c1a3094b279521bef667c33ca06a617120da06d6",
        "tarball": "https://registry.npmjs.org/node-mysql/-/node-mysql-0.4.2.tgz"
    },
    "gitHead": "9fe54677bb6d4467013a2208a7d14bd73a544da8",
    "homepage": "https://github.com/redblaze/node-mysql",
    "jam": {
        "main": "lib/node-mysql.js",
        "include": [
            "lib/node-mysql.js",
            "README.md",
            "LICENSE"
        ]
    },
    "licenses": [
        {
            "type": "MIT",
            "url": "https://github.com/redblaze/node-mysql/raw/master/LICENSE"
        }
    ],
    "main": "./lib/node-mysql",
    "maintainers": [
        {
            "name": "redblaze",
            "email": "redblaze2005@gmail.com"
        }
    ],
    "name": "node-mysql",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/redblaze/node-mysql.git"
    },
    "scripts": {},
    "version": "0.4.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module node-mysql](#apidoc.module.node-mysql)
1.  [function <span class="apidocSignatureSpan">node-mysql.</span>DB ()](#apidoc.element.node-mysql.DB)
1.  [function <span class="apidocSignatureSpan">node-mysql.</span>Row ()](#apidoc.element.node-mysql.Row)
1.  [function <span class="apidocSignatureSpan">node-mysql.</span>Table ()](#apidoc.element.node-mysql.Table)
1.  [function <span class="apidocSignatureSpan">node-mysql.</span>db ()](#apidoc.element.node-mysql.db)
1.  object <span class="apidocSignatureSpan">node-mysql.</span>DB.prototype
1.  object <span class="apidocSignatureSpan">node-mysql.</span>Row.prototype
1.  object <span class="apidocSignatureSpan">node-mysql.</span>Table.prototype
1.  object <span class="apidocSignatureSpan">node-mysql.</span>db.prototype
1.  object <span class="apidocSignatureSpan">node-mysql.</span>model
1.  string <span class="apidocSignatureSpan">node-mysql.</span>OPTIMISTIC_LOCK_EXCEPTION

#### [module node-mysql.DB](#apidoc.module.node-mysql.DB)
1.  [function <span class="apidocSignatureSpan">node-mysql.</span>DB ()](#apidoc.element.node-mysql.DB.DB)
1.  [function <span class="apidocSignatureSpan">node-mysql.DB.</span>format (str, bindings)](#apidoc.element.node-mysql.DB.format)

#### [module node-mysql.DB.prototype](#apidoc.module.node-mysql.DB.prototype)
1.  [function <span class="apidocSignatureSpan">node-mysql.DB.prototype.</span>_init ()](#apidoc.element.node-mysql.DB.prototype._init)
1.  [function <span class="apidocSignatureSpan">node-mysql.DB.prototype.</span>add ()](#apidoc.element.node-mysql.DB.prototype.add)
1.  [function <span class="apidocSignatureSpan">node-mysql.DB.prototype.</span>clone ()](#apidoc.element.node-mysql.DB.prototype.clone)
1.  [function <span class="apidocSignatureSpan">node-mysql.DB.prototype.</span>extend ()](#apidoc.element.node-mysql.DB.prototype.extend)
1.  [function <span class="apidocSignatureSpan">node-mysql.DB.prototype.</span>get ()](#apidoc.element.node-mysql.DB.prototype.get)

#### [module node-mysql.Row](#apidoc.module.node-mysql.Row)
1.  [function <span class="apidocSignatureSpan">node-mysql.</span>Row ()](#apidoc.element.node-mysql.Row.Row)

#### [module node-mysql.Row.prototype](#apidoc.module.node-mysql.Row.prototype)
1.  [function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>_getVersion ()](#apidoc.element.node-mysql.Row.prototype._getVersion)
1.  [function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>_init (data, cfg)](#apidoc.element.node-mysql.Row.prototype._init)
1.  [function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>_load (conn, name, cb)](#apidoc.element.node-mysql.Row.prototype._load)
1.  [function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>_nextVersion ()](#apidoc.element.node-mysql.Row.prototype._nextVersion)
1.  [function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>_refineDtoForUpdate (dto)](#apidoc.element.node-mysql.Row.prototype._refineDtoForUpdate)
1.  [function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>_update (conn, dto, conditions, cb)](#apidoc.element.node-mysql.Row.prototype._update)
1.  [function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>_updateLocalData (dto)](#apidoc.element.node-mysql.Row.prototype._updateLocalData)
1.  [function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>get (fieldName)](#apidoc.element.node-mysql.Row.prototype.get)
1.  [function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>getId ()](#apidoc.element.node-mysql.Row.prototype.getId)
1.  [function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>linkedBy (conn, name, cb)](#apidoc.element.node-mysql.Row.prototype.linkedBy)
1.  [function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>linksTo (conn, name, cb)](#apidoc.element.node-mysql.Row.prototype.linksTo)
1.  [function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>load (conn, name, cb)](#apidoc.element.node-mysql.Row.prototype.load)
1.  [function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>relatesTo (conn, name, cb)](#apidoc.element.node-mysql.Row.prototype.relatesTo)
1.  [function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>update (conn, dto, cb)](#apidoc.element.node-mysql.Row.prototype.update)
1.  [function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>updateWithoutOptimisticLock (conn, dto, cb)](#apidoc.element.node-mysql.Row.prototype.updateWithoutOptimisticLock)

#### [module node-mysql.Table](#apidoc.module.node-mysql.Table)
1.  [function <span class="apidocSignatureSpan">node-mysql.</span>Table ()](#apidoc.element.node-mysql.Table.Table)

#### [module node-mysql.Table.prototype](#apidoc.module.node-mysql.Table.prototype)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_create (conn, dto, cb)](#apidoc.element.node-mysql.Table.prototype._create)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_hasUpdatableField (field)](#apidoc.element.node-mysql.Table.prototype._hasUpdatableField)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_init (cfg)](#apidoc.element.node-mysql.Table.prototype._init)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_lookupLinkedByMap (name)](#apidoc.element.node-mysql.Table.prototype._lookupLinkedByMap)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_lookupLinksToMap (name)](#apidoc.element.node-mysql.Table.prototype._lookupLinksToMap)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_lookupRelatesToMap (name)](#apidoc.element.node-mysql.Table.prototype._lookupRelatesToMap)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_refineDto (dto, autoId)](#apidoc.element.node-mysql.Table.prototype._refineDto)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_refineDtoForCreate (dto)](#apidoc.element.node-mysql.Table.prototype._refineDtoForCreate)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>baseQuery (str, bindings)](#apidoc.element.node-mysql.Table.prototype.baseQuery)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>clone (conn, dto, cb)](#apidoc.element.node-mysql.Table.prototype.clone)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>create (conn, dto, cb)](#apidoc.element.node-mysql.Table.prototype.create)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>find (conn, q, cb)](#apidoc.element.node-mysql.Table.prototype.find)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>findAll (conn, cb)](#apidoc.element.node-mysql.Table.prototype.findAll)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>findById (conn, id, cb)](#apidoc.element.node-mysql.Table.prototype.findById)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>findFirst (conn, q, cb)](#apidoc.element.node-mysql.Table.prototype.findFirst)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>getCreatedFieldName ()](#apidoc.element.node-mysql.Table.prototype.getCreatedFieldName)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>getIdFieldName ()](#apidoc.element.node-mysql.Table.prototype.getIdFieldName)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>getName ()](#apidoc.element.node-mysql.Table.prototype.getName)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>getUpdatedFieldName ()](#apidoc.element.node-mysql.Table.prototype.getUpdatedFieldName)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>getVersionFieldName ()](#apidoc.element.node-mysql.Table.prototype.getVersionFieldName)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>linkedBy (cfg)](#apidoc.element.node-mysql.Table.prototype.linkedBy)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>linksTo (cfg)](#apidoc.element.node-mysql.Table.prototype.linksTo)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>lockById (conn, id, cb)](#apidoc.element.node-mysql.Table.prototype.lockById)
1.  [function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>relatesTo (cfg)](#apidoc.element.node-mysql.Table.prototype.relatesTo)

#### [module node-mysql.db](#apidoc.module.node-mysql.db)
1.  [function <span class="apidocSignatureSpan">node-mysql.</span>db ()](#apidoc.element.node-mysql.db.db)
1.  [function <span class="apidocSignatureSpan">node-mysql.db.</span>format (str, bindings)](#apidoc.element.node-mysql.db.format)

#### [module node-mysql.db.prototype](#apidoc.module.node-mysql.db.prototype)
1.  [function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>_buildCfg (cfg, override)](#apidoc.element.node-mysql.db.prototype._buildCfg)
1.  [function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>_connect (pool, proc, cb)](#apidoc.element.node-mysql.db.prototype._connect)
1.  [function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>_enterTransaction (conn)](#apidoc.element.node-mysql.db.prototype._enterTransaction)
1.  [function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>_init (cfg)](#apidoc.element.node-mysql.db.prototype._init)
1.  [function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>_isTxnConnection (conn)](#apidoc.element.node-mysql.db.prototype._isTxnConnection)
1.  [function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>_leaveTransaction (conn)](#apidoc.element.node-mysql.db.prototype._leaveTransaction)
1.  [function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>_prepare (cb)](#apidoc.element.node-mysql.db.prototype._prepare)
1.  [function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>connect (proc, cb)](#apidoc.element.node-mysql.db.prototype.connect)
1.  [function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>cursor (q, proc, _cb)](#apidoc.element.node-mysql.db.prototype.cursor)
1.  [function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>end ()](#apidoc.element.node-mysql.db.prototype.end)
1.  [function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>getConnection (cb)](#apidoc.element.node-mysql.db.prototype.getConnection)
1.  [function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>transaction (conn, proc, cb)](#apidoc.element.node-mysql.db.prototype.transaction)

#### [module node-mysql.model](#apidoc.module.node-mysql.model)
1.  [function <span class="apidocSignatureSpan">node-mysql.model.</span>Row ()](#apidoc.element.node-mysql.model.Row)
1.  [function <span class="apidocSignatureSpan">node-mysql.model.</span>Table ()](#apidoc.element.node-mysql.model.Table)
1.  string <span class="apidocSignatureSpan">node-mysql.model.</span>OPTIMISTIC_LOCK_EXCEPTION



# <a name="apidoc.module.node-mysql"></a>[module node-mysql](#apidoc.module.node-mysql)

#### <a name="apidoc.element.node-mysql.DB"></a>[function <span class="apidocSignatureSpan">node-mysql.</span>DB ()](#apidoc.element.node-mysql.DB)
- description and source-code
```javascript
DB = function () {
    this._init.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mysql.Row"></a>[function <span class="apidocSignatureSpan">node-mysql.</span>Row ()](#apidoc.element.node-mysql.Row)
- description and source-code
```javascript
Row = function () {
    this._init.apply(this, arguments);
}
```
- example usage
```shell
...
var q = 'select * from users';

db.cursor(q, function(row, cb) {
    cps.rescur({
        'try': function() {
            cps.seq([
                function(_, cb) {
                    var user = new User.Row(row);
                    user.update(conn, {active: 1}, cb);
                },
                function(res, cb) {
                    console.log(res);
                    cb();
                }
            ], cb);
...
```

#### <a name="apidoc.element.node-mysql.Table"></a>[function <span class="apidocSignatureSpan">node-mysql.</span>Table ()](#apidoc.element.node-mysql.Table)
- description and source-code
```javascript
Table = function () {
    this._init.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mysql.db"></a>[function <span class="apidocSignatureSpan">node-mysql.</span>db ()](#apidoc.element.node-mysql.db)
- description and source-code
```javascript
db = function () {
    this._init.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-mysql.DB"></a>[module node-mysql.DB](#apidoc.module.node-mysql.DB)

#### <a name="apidoc.element.node-mysql.DB.DB"></a>[function <span class="apidocSignatureSpan">node-mysql.</span>DB ()](#apidoc.element.node-mysql.DB.DB)
- description and source-code
```javascript
DB = function () {
    this._init.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mysql.DB.format"></a>[function <span class="apidocSignatureSpan">node-mysql.DB.</span>format (str, bindings)](#apidoc.element.node-mysql.DB.format)
- description and source-code
```javascript
format = function (str, bindings) {
    var l = str.split('?')

    if (l.length - 1 != bindings.length) {
        throw new Error('sql string format error');
    }

    var res = [];

    for (var i = 0; i < bindings.length; i++) {
        res.push(l[i]);
        res.push(mysql.escape(bindings[i]));
    }

    res.push(l[l.length - 1]);

    return res.join(' ');
}
```
- example usage
```shell
...
        }
    ], cb);
}, cb);
'''


<a name="DB-format" />
### DB.format(query_string, variable_bindings)

This is a wrapper of the query string formatting functionality
provided by the mysql package.  Note that this is a global static
method defined on the class DB.  It is NOT an instance method defined
a a DB instance db.

__Example__
...
```



# <a name="apidoc.module.node-mysql.DB.prototype"></a>[module node-mysql.DB.prototype](#apidoc.module.node-mysql.DB.prototype)

#### <a name="apidoc.element.node-mysql.DB.prototype._init"></a>[function <span class="apidocSignatureSpan">node-mysql.DB.prototype.</span>_init ()](#apidoc.element.node-mysql.DB.prototype._init)
- description and source-code
```javascript
_init = function () {
    var tmp = this.parent;
    this.parent = superclass.prototype;
    var res = fn.apply(this, arguments);
    this.parent = tmp;
    return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mysql.DB.prototype.add"></a>[function <span class="apidocSignatureSpan">node-mysql.DB.prototype.</span>add ()](#apidoc.element.node-mysql.DB.prototype.add)
- description and source-code
```javascript
add = function () {
    var tmp = this.parent;
    this.parent = superclass.prototype;
    var res = fn.apply(this, arguments);
    this.parent = tmp;
    return res;
}
```
- example usage
```shell
...
<a name="db-end" />
### db.end();

This function destructs the db object.

<a name="db-add"/>

### db.add(config);

This function is used to define a model that belongs to the db object.  The model config object is of the following format:

'''json
{
"name": {
    "type": "String",
...
```

#### <a name="apidoc.element.node-mysql.DB.prototype.clone"></a>[function <span class="apidocSignatureSpan">node-mysql.DB.prototype.</span>clone ()](#apidoc.element.node-mysql.DB.prototype.clone)
- description and source-code
```javascript
clone = function () {
    var tmp = this.parent;
    this.parent = superclass.prototype;
    var res = fn.apply(this, arguments);
    this.parent = tmp;
    return res;
}
```
- example usage
```shell
...
* version

All of the these fields will be filled by the invocation to table.create.


<a name="table-clone"/>

### table.clone(database_connection, data_object, callback)

This API is very similar to table.create.  The key difference is that
it does not mask out any data field carried in data_object.  Instead,
it literally uses every thing in data_object to create a new row.  In
other words, it'll honor the values of the following fields in
data_object:
...
```

#### <a name="apidoc.element.node-mysql.DB.prototype.extend"></a>[function <span class="apidocSignatureSpan">node-mysql.DB.prototype.</span>extend ()](#apidoc.element.node-mysql.DB.prototype.extend)
- description and source-code
```javascript
extend = function () {
    var tmp = this.parent;
    this.parent = superclass.prototype;
    var res = fn.apply(this, arguments);
    this.parent = tmp;
    return res;
}
```
- example usage
```shell
...
        _buildCfg: function(cfg, override) {
var res = {};

for (var k in cfg) {
    res[k] = cfg[k];
}

$U.extend(res, override);
return res;
        },

        connect: function(proc, cb) {
var me = this;

cps.seq([
...
```

#### <a name="apidoc.element.node-mysql.DB.prototype.get"></a>[function <span class="apidocSignatureSpan">node-mysql.DB.prototype.</span>get ()](#apidoc.element.node-mysql.DB.prototype.get)
- description and source-code
```javascript
get = function () {
    var tmp = this.parent;
    this.parent = superclass.prototype;
    var res = fn.apply(this, arguments);
    this.parent = tmp;
    return res;
}
```
- example usage
```shell
...
* We created a model for the table "orders" in the database.
* We add a method getFirstOrderItem into the Row class of this model.
* We add a method createOrderWithCoupon into the Table class of this model.
* We follow the foreign key relations of the "orders" table to define some link relations.

<a name="db-get"/>

### db.get(table_name)

Once you use db.add to create a model in the db object, you can then
use db.get to retrieve it by name.  The return value of
db.get if a object of the following format:

'''json
{
...
```



# <a name="apidoc.module.node-mysql.Row"></a>[module node-mysql.Row](#apidoc.module.node-mysql.Row)

#### <a name="apidoc.element.node-mysql.Row.Row"></a>[function <span class="apidocSignatureSpan">node-mysql.</span>Row ()](#apidoc.element.node-mysql.Row.Row)
- description and source-code
```javascript
Row = function () {
    this._init.apply(this, arguments);
}
```
- example usage
```shell
...
var q = 'select * from users';

db.cursor(q, function(row, cb) {
    cps.rescur({
        'try': function() {
            cps.seq([
                function(_, cb) {
                    var user = new User.Row(row);
                    user.update(conn, {active: 1}, cb);
                },
                function(res, cb) {
                    console.log(res);
                    cb();
                }
            ], cb);
...
```



# <a name="apidoc.module.node-mysql.Row.prototype"></a>[module node-mysql.Row.prototype](#apidoc.module.node-mysql.Row.prototype)

#### <a name="apidoc.element.node-mysql.Row.prototype._getVersion"></a>[function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>_getVersion ()](#apidoc.element.node-mysql.Row.prototype._getVersion)
- description and source-code
```javascript
_getVersion = function () {
    return this._data[this._table.getVersionFieldName()];
}
```
- example usage
```shell
...
this._update(conn, dto, null, cb);
        },

        update: function(conn, dto, cb) {
var me = this;

dto['version'] = this._nextVersion();
var cond = DB.format('version = ?', [this._getVersion()]);

cps.seq([
    function(_, cb) {
        me._update(conn, dto, cond, cb);
    },
    function(res, cb) {
        if (res.changedRows === 0) {
...
```

#### <a name="apidoc.element.node-mysql.Row.prototype._init"></a>[function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>_init (data, cfg)](#apidoc.element.node-mysql.Row.prototype._init)
- description and source-code
```javascript
_init = function (data, cfg) {
    this._table = cfg.table;
    this._data = data;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mysql.Row.prototype._load"></a>[function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>_load (conn, name, cb)](#apidoc.element.node-mysql.Row.prototype._load)
- description and source-code
```javascript
_load = function (conn, name, cb) {
    var cfg = this._table._lookupLinksToMap(name);
    if (cfg) {
        return this.linksTo(conn, name, cb);
    }

    var cfg = this._table._lookupLinkedByMap(name);
    if (cfg) {
        return this.linkedBy(conn, name, cb);
    }

    var cfg = this._table._lookupRelatesToMap(name);
    if (cfg) {
        return this.relatesTo(conn, name, cb);
    }

    throw new Error('no linksTo or linkedBy or relatesTo: ' + name + ' defined on: ' + this._table.getName());
}
```
- example usage
```shell
...
        },

        load: function(conn, name, cb) {
var value = this.get(name);
if (value) {
    cb(null, value);
} else {
    this._load(conn, name, cb);
}
        },

        linksTo: function(conn, name, cb) {
var me = this;

var cfg = this._table._lookupLinksToMap(name);
...
```

#### <a name="apidoc.element.node-mysql.Row.prototype._nextVersion"></a>[function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>_nextVersion ()](#apidoc.element.node-mysql.Row.prototype._nextVersion)
- description and source-code
```javascript
_nextVersion = function () {
    return this._data[this._table.getVersionFieldName()] + 1;
}
```
- example usage
```shell
...
        updateWithoutOptimisticLock: function(conn, dto, cb) {
this._update(conn, dto, null, cb);
        },

        update: function(conn, dto, cb) {
var me = this;

dto['version'] = this._nextVersion();
var cond = DB.format('version = ?', [this._getVersion()]);

cps.seq([
    function(_, cb) {
        me._update(conn, dto, cond, cb);
    },
    function(res, cb) {
...
```

#### <a name="apidoc.element.node-mysql.Row.prototype._refineDtoForUpdate"></a>[function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>_refineDtoForUpdate (dto)](#apidoc.element.node-mysql.Row.prototype._refineDtoForUpdate)
- description and source-code
```javascript
_refineDtoForUpdate = function (dto) {

    var res = {};

    for (var k in dto) {
        if (this._table._hasUpdatableField(k)) {
            res[k] = dto[k];
        }
    }

    var d = new Date();
    res[this._table.getUpdatedFieldName()] = d;

    return res;
}
```
- example usage
```shell
...
], cb);
        },

        _update: function(conn, dto, conditions, cb) {
var me = this;

// dto[this._table.getUpdatedFieldName()] = new Date();
dto = this._refineDtoForUpdate(dto);

var l = [
    ' update ', this._table.getName(), ' set '
];

var first = true;
for (var k in dto) {
...
```

#### <a name="apidoc.element.node-mysql.Row.prototype._update"></a>[function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>_update (conn, dto, conditions, cb)](#apidoc.element.node-mysql.Row.prototype._update)
- description and source-code
```javascript
_update = function (conn, dto, conditions, cb) {
    var me = this;

    // dto[this._table.getUpdatedFieldName()] = new Date();
    dto = this._refineDtoForUpdate(dto);

    var l = [
        ' update ', this._table.getName(), ' set '
    ];

    var first = true;
    for (var k in dto) {
        var v = dto[k];
        if (first) {
            first = false;
        } else {
            l.push(', ');
        }
        l.push(
            ' ', k, ' = ', conn.escape(v)
        );
    }

    l.push(
        ' where ', this._table.getIdFieldName(), ' = ', this.getId()
    );

    if (conditions) {
        l.push(
            ' and ', conditions
        );
    }

    l.push(' ; ');

    var q = l.join('');

    // console.log(q);

    cps.seq([
        function(_, cb) {
            conn.query(q, cb);
        },
        function(res, cb) {
            me._updateLocalData(dto);
            cb(null, res);
        }
    ], cb);
}
```
- example usage
```shell
...
var d = new Date();
res[this._table.getUpdatedFieldName()] = d;

return res;
        },

        updateWithoutOptimisticLock: function(conn, dto, cb) {
this._update(conn, dto, null, cb);
        },

        update: function(conn, dto, cb) {
var me = this;

dto['version'] = this._nextVersion();
var cond = DB.format('version = ?', [this._getVersion()]);
...
```

#### <a name="apidoc.element.node-mysql.Row.prototype._updateLocalData"></a>[function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>_updateLocalData (dto)](#apidoc.element.node-mysql.Row.prototype._updateLocalData)
- description and source-code
```javascript
_updateLocalData = function (dto) {
    for (var k in dto) {
        var v = dto[k];
        this._data[k] = v;
    }
}
```
- example usage
```shell
...
    // console.log(q);

    cps.seq([
        function(_, cb) {
            conn.query(q, cb);
        },
        function(res, cb) {
            me._updateLocalData(dto);
            cb(null, res);
        }
    ], cb);
},

get: function(fieldName) {
    return this._data[fieldName]
...
```

#### <a name="apidoc.element.node-mysql.Row.prototype.get"></a>[function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>get (fieldName)](#apidoc.element.node-mysql.Row.prototype.get)
- description and source-code
```javascript
get = function (fieldName) {
    return this._data[fieldName]
}
```
- example usage
```shell
...
* We created a model for the table "orders" in the database.
* We add a method getFirstOrderItem into the Row class of this model.
* We add a method createOrderWithCoupon into the Table class of this model.
* We follow the foreign key relations of the "orders" table to define some link relations.

<a name="db-get"/>

### db.get(table_name)

Once you use db.add to create a model in the db object, you can then
use db.get to retrieve it by name.  The return value of
db.get if a object of the following format:

'''json
{
...
```

#### <a name="apidoc.element.node-mysql.Row.prototype.getId"></a>[function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>getId ()](#apidoc.element.node-mysql.Row.prototype.getId)
- description and source-code
```javascript
getId = function () {
    return this._data[this._table.getIdFieldName()];
}
```
- example usage
```shell
...
                cb(null, items[0]);
            }
        ], cb);
    }
},
Table: {
    createOrderUsingCoupon: function(conn, dto, coupon, cb) {
        dto['coupon_id'] = coupon.getId();
        this.create(conn, dto, cb);
    }
}
})
.linkedBy({
    name: 'items',
    key: 'order_id',
...
```

#### <a name="apidoc.element.node-mysql.Row.prototype.linkedBy"></a>[function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>linkedBy (conn, name, cb)](#apidoc.element.node-mysql.Row.prototype.linkedBy)
- description and source-code
```javascript
linkedBy = function (conn, name, cb) {
    var me = this;

    var cfg = this._table._lookupLinkedByMap(name);

    if (cfg) {
        var otherTable = this._table._db.get(cfg.table).Table;
        return cps.seq([
            function(_, cb) {
                otherTable.find(conn, otherTable.baseQuery('where ' + cfg.key + ' = ?', [me.getId()]), cb);
            },
            function(res, cb) {
                me._data[cfg.name] = res;
                cb(null, me._data[cfg.name]);
            }
        ], cb);
    } else {
        throw new Error('no linkedBy: ' + name + ' defined on: ' + this._table.getName());
    }
}
```
- example usage
```shell
...
idFieldName: 'order_id',
Row: {
    getFirstOrderItem: function(conn, cb) {
        var me = this;

        cps.seq([
            function(_, cb) {
                me.linkedBy(conn, 'items', cb);
            },
            function(items, cb) {
                cb(null, items[0]);
            }
        ], cb);
    }
},
...
```

#### <a name="apidoc.element.node-mysql.Row.prototype.linksTo"></a>[function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>linksTo (conn, name, cb)](#apidoc.element.node-mysql.Row.prototype.linksTo)
- description and source-code
```javascript
linksTo = function (conn, name, cb) {
    var me = this;

    var cfg = this._table._lookupLinksToMap(name);

    if (cfg) {
        var otherTable = this._table._db.get(cfg.table).Table;
        return cps.seq([
            function(_, cb) {
                otherTable.findById(conn, me.get(cfg.key), cb);
            },
            function(res, cb) {
                me._data[cfg.name] = res;
                cb(null, res);
            }
        ], cb);
    } else {
        throw new Error('no linksTo: ' + name + ' defined on: ' + this._table.getName());
    }
}
```
- example usage
```shell
...
}
})
.linkedBy({
    name: 'items',
    key: 'order_id',
    table: 'order_items'
})
.linksTo({
    name: 'user',
    key: 'user_id',
    table: 'users'
})
.linksTo({
    name: 'coupon',
    key: 'coupon_id',
...
```

#### <a name="apidoc.element.node-mysql.Row.prototype.load"></a>[function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>load (conn, name, cb)](#apidoc.element.node-mysql.Row.prototype.load)
- description and source-code
```javascript
load = function (conn, name, cb) {
    var value = this.get(name);
    if (value) {
        cb(null, value);
    } else {
        this._load(conn, name, cb);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mysql.Row.prototype.relatesTo"></a>[function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>relatesTo (conn, name, cb)](#apidoc.element.node-mysql.Row.prototype.relatesTo)
- description and source-code
```javascript
relatesTo = function (conn, name, cb) {
    var me = this;

    var cfg = this._table._lookupRelatesToMap(name);
    if (cfg) {
        var otherTable = this._table._db.get(cfg.table).Table;
        var throughTable = this._table._db.get(cfg.through).Table;

        return cps.seq([
            function(_, cb) {
                var _q = 'select t.* from ' +
                        otherTable.getName()  + ' t, ' +
                        throughTable.getName() + ' r where ' +
                        'r.' + cfg['leftKey'] + ' = ? and ' +
                        'r.' + cfg['rightKey'] + ' = t.' + otherTable.getIdFieldName()
                    ;
                var q = DB.format(_q, [me.getId()]);
                otherTable.find(conn, q, cb);
            },
            function(res, cb) {
                me._data[cfg.name] = res;
                cb(null, me._data[cfg.name]);
            }
        ], cb);
    } else {
        throw new Error('no relatesTo: ' + name + ' defined on: ' + this._table.getName());
    }
}
```
- example usage
```shell
...

Once a "linkedBy" is set up on a table, a row object corresponding to
this table can call the "linkedBy" method to pull more (associated)
data into the row.  See examples [here](#row-linkedBy).

<a name="table-relatesTo"/>

### table.relatesTo(config)

The config object has the following schema:

'''json
{
"name": {
    "type": "String",
...
```

#### <a name="apidoc.element.node-mysql.Row.prototype.update"></a>[function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>update (conn, dto, cb)](#apidoc.element.node-mysql.Row.prototype.update)
- description and source-code
```javascript
update = function (conn, dto, cb) {
    var me = this;

    dto['version'] = this._nextVersion();
    var cond = DB.format('version = ?', [this._getVersion()]);

    cps.seq([
        function(_, cb) {
            me._update(conn, dto, cond, cb);
        },
        function(res, cb) {
            if (res.changedRows === 0) {
                throw new Error(Model.OPTIMISTIC_LOCK_EXCEPTION);
            } else {
                cb(null, res);
            }
        }
    ], cb);
}
```
- example usage
```shell
...

        db.cursor(q, function(row, cb) {
cps.rescur({
    'try': function() {
        cps.seq([
            function(_, cb) {
                var user = new User.Row(row);
                user.update(conn, {active: 1}, cb);
            },
            function(res, cb) {
                console.log(res);
                cb();
            }
        ], cb);
    },
...
```

#### <a name="apidoc.element.node-mysql.Row.prototype.updateWithoutOptimisticLock"></a>[function <span class="apidocSignatureSpan">node-mysql.Row.prototype.</span>updateWithoutOptimisticLock (conn, dto, cb)](#apidoc.element.node-mysql.Row.prototype.updateWithoutOptimisticLock)
- description and source-code
```javascript
updateWithoutOptimisticLock = function (conn, dto, cb) {
    this._update(conn, dto, null, cb);
}
```
- example usage
```shell
...
            }
        ], cb);
    }, cb);
};
'''

<a name="row-updateWithoutOptimisticLock"/>
### row.updateWithoutOptimisticLock(database_connection, update_object, callback)

This function is the same as row.update with only one difference: it
does not care about the optimistic lock version field.  It neither
looks at this field nor update field.  This might be useful
ocasionally when optimistic lock functionality needs to be overriden.
...
```



# <a name="apidoc.module.node-mysql.Table"></a>[module node-mysql.Table](#apidoc.module.node-mysql.Table)

#### <a name="apidoc.element.node-mysql.Table.Table"></a>[function <span class="apidocSignatureSpan">node-mysql.</span>Table ()](#apidoc.element.node-mysql.Table.Table)
- description and source-code
```javascript
Table = function () {
    this._init.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-mysql.Table.prototype"></a>[module node-mysql.Table.prototype](#apidoc.module.node-mysql.Table.prototype)

#### <a name="apidoc.element.node-mysql.Table.prototype._create"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_create (conn, dto, cb)](#apidoc.element.node-mysql.Table.prototype._create)
- description and source-code
```javascript
_create = function (conn, dto, cb) {
    var me = this;

    var l = [
        ' insert into ' + this.getName() + ' set '
    ];

    var first = true;

    $U.each(dto, function(v, k) {
        if (first) {
            first = false;
        } else {
            l.push(', ');
        }
        l.push(
            ' ', k, ' = ', conn.escape(v)
        );
    });

    l.push(' ; ');

    var q = l.join('');

    // console.log(q);

    cps.seq([
        function(_, cb) {
            conn.query(q, cb);
        },
        function(res, cb) {
            dto[me._idFieldName] = res.insertId;
            cb(null, new me._rowClass(dto));
        }
    ], cb);
}
```
- example usage
```shell
...
res[this.getVersionFieldName()] = 0;

return res;
        },

        create: function(conn, dto, cb) {
dto = this._refineDtoForCreate(dto);
this._create(conn, dto, cb);
        },

        _create: function(conn, dto, cb) {
var me = this;

var l = [
    ' insert into ' + this.getName() + ' set '
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype._hasUpdatableField"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_hasUpdatableField (field)](#apidoc.element.node-mysql.Table.prototype._hasUpdatableField)
- description and source-code
```javascript
_hasUpdatableField = function (field) {
    if (field == this.getIdFieldName()) {
        return false;
    }
    if (field == this.getCreatedFieldName()) {
        return false;
    }
    var schema = this._db._schema[this.getName()];
    return $U.contains(schema, field);
}
```
- example usage
```shell
...
        },

        _refineDtoForUpdate: function(dto) {

var res = {};

for (var k in dto) {
    if (this._table._hasUpdatableField(k)) {
        res[k] = dto[k];
    }
}

var d = new Date();
res[this._table.getUpdatedFieldName()] = d;
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype._init"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_init (cfg)](#apidoc.element.node-mysql.Table.prototype._init)
- description and source-code
```javascript
_init = function (cfg) {
    this._name = cfg.name;
    this._idFieldName = cfg.idFieldName || 'id';
    this._versionFieldName = cfg.versionFieldName || 'version';
    this._createdFieldName = cfg.createdFieldName || 'date_created';
    this._updatedFieldName = cfg.updatedFieldName || 'last_updated';

    this._rowClass = cfg['rowClass'];
    // this._schema = cfg['schema'];
    this._db = cfg['db'];

    this._linksToMap = {};
    this._linkedByMap = {};
    this._relatesToMap = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mysql.Table.prototype._lookupLinkedByMap"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_lookupLinkedByMap (name)](#apidoc.element.node-mysql.Table.prototype._lookupLinkedByMap)
- description and source-code
```javascript
_lookupLinkedByMap = function (name) {
    var cfg = this._linkedByMap[name];
    if (cfg) {
        cfg.name = name;
    }
    return cfg;
}
```
- example usage
```shell
...

        _load: function(conn, name, cb) {
var cfg = this._table._lookupLinksToMap(name);
if (cfg) {
    return this.linksTo(conn, name, cb);
}

var cfg = this._table._lookupLinkedByMap(name);
if (cfg) {
    return this.linkedBy(conn, name, cb);
}

var cfg = this._table._lookupRelatesToMap(name);
if (cfg) {
    return this.relatesTo(conn, name, cb);
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype._lookupLinksToMap"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_lookupLinksToMap (name)](#apidoc.element.node-mysql.Table.prototype._lookupLinksToMap)
- description and source-code
```javascript
_lookupLinksToMap = function (name) {
    var cfg = this._linksToMap[name];
    if (cfg) {
        cfg.name = name;
    }
    return cfg;
}
```
- example usage
```shell
...
        },

        get: function(fieldName) {
return this._data[fieldName]
        },

        _load: function(conn, name, cb) {
var cfg = this._table._lookupLinksToMap(name);
if (cfg) {
    return this.linksTo(conn, name, cb);
}

var cfg = this._table._lookupLinkedByMap(name);
if (cfg) {
    return this.linkedBy(conn, name, cb);
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype._lookupRelatesToMap"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_lookupRelatesToMap (name)](#apidoc.element.node-mysql.Table.prototype._lookupRelatesToMap)
- description and source-code
```javascript
_lookupRelatesToMap = function (name) {
    var cfg = this._relatesToMap[name];
    if (cfg) {
        cfg.name = name;
    }
    return cfg;
}
```
- example usage
```shell
...
    }

    var cfg = this._table._lookupLinkedByMap(name);
    if (cfg) {
        return this.linkedBy(conn, name, cb);
    }

    var cfg = this._table._lookupRelatesToMap(name);
    if (cfg) {
        return this.relatesTo(conn, name, cb);
    }

    throw new Error('no linksTo or linkedBy or relatesTo: ' + name + ' defined on: ' + this._table.getName());
},
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype._refineDto"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_refineDto (dto, autoId)](#apidoc.element.node-mysql.Table.prototype._refineDto)
- description and source-code
```javascript
_refineDto = function (dto, autoId) {
    autoId = (autoId === undefined)? true: autoId;
    var res = {};

    var schema = this._db._schema[this.getName()];
    $U.each(schema, function(field) {
        res[field] = dto[field];
    });

    if (autoId) {
        delete res[this.getIdFieldName()];
    }

    return res;
}
```
- example usage
```shell
...
    delete res[this.getIdFieldName()];
}

return res;
        },

        _refineDtoForCreate: function(dto) {
var res = this._refineDto(dto);

var d = new Date();
res[this.getCreatedFieldName()] = d;
res[this.getUpdatedFieldName()] = d;
res[this.getVersionFieldName()] = 0;

return res;
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype._refineDtoForCreate"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>_refineDtoForCreate (dto)](#apidoc.element.node-mysql.Table.prototype._refineDtoForCreate)
- description and source-code
```javascript
_refineDtoForCreate = function (dto) {
    var res = this._refineDto(dto);

    var d = new Date();
    res[this.getCreatedFieldName()] = d;
    res[this.getUpdatedFieldName()] = d;
    res[this.getVersionFieldName()] = 0;

    return res;
}
```
- example usage
```shell
...
res[this.getUpdatedFieldName()] = d;
res[this.getVersionFieldName()] = 0;

return res;
        },

        create: function(conn, dto, cb) {
dto = this._refineDtoForCreate(dto);
this._create(conn, dto, cb);
        },

        _create: function(conn, dto, cb) {
var me = this;

var l = [
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype.baseQuery"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>baseQuery (str, bindings)](#apidoc.element.node-mysql.Table.prototype.baseQuery)
- description and source-code
```javascript
baseQuery = function (str, bindings) {
    var q = ' select * from ' + this.getName() + ' ';
    var further;

    if (str != null) {
        if (bindings == null) {
            further = str;
        } else {
            further = DB.format(str, bindings);
        }
    }

    if (further != null) {
        q += further;
    }
    return q;
}
```
- example usage
```shell
...

<a name="table-findAll"/>
### table.findAll(database_connection, callback)

This finds all the rows in a table.

<a name="table-baseQuery"/>
### table.baseQuery(query_string, variable_bindings)

This is a short-hand for:

'''javascript
DB.format('select * from table_name' + query_string, variable_bindings);
'''
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype.clone"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>clone (conn, dto, cb)](#apidoc.element.node-mysql.Table.prototype.clone)
- description and source-code
```javascript
clone = function (conn, dto, cb) {
    dto = this._refineDto(dto, false);
    this._create(conn, dto, cb);
}
```
- example usage
```shell
...
* version

All of the these fields will be filled by the invocation to table.create.


<a name="table-clone"/>

### table.clone(database_connection, data_object, callback)

This API is very similar to table.create.  The key difference is that
it does not mask out any data field carried in data_object.  Instead,
it literally uses every thing in data_object to create a new row.  In
other words, it'll honor the values of the following fields in
data_object:
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype.create"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>create (conn, dto, cb)](#apidoc.element.node-mysql.Table.prototype.create)
- description and source-code
```javascript
create = function (conn, dto, cb) {
    dto = this._refineDtoForCreate(dto);
    this._create(conn, dto, cb);
}
```
- example usage
```shell
...
function(
    conn/*A new transactional connection is
          created to handle the transactional session.*/,
    cb
) {
    cps.seq([
        function(_, cb) {
            Model.Table.create(conn, getSampleDto(), cb);
        },
        function(_, cb) {
            dw.transaction(
                conn/*This is already a transactional connection.*/,
                function(
                    conn/*No new transactional connection created.
                          This connection is the same one as
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype.find"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>find (conn, q, cb)](#apidoc.element.node-mysql.Table.prototype.find)
- description and source-code
```javascript
find = function (conn, q, cb) {
    var me = this;

    cps.seq([
        function(_, cb) {
            conn.query(q, cb);
        },
        function(res, cb) {
            cb(null, $U.map(res, function(o) {
                return new me._rowClass(o);
            }));
        }
    ], cb);
}
```
- example usage
```shell
...
* last_udpated
* version

This API can be useful when one attempts to clone a row in a table
literally to another table (which might be in another database).

<a name="table-find"/>
### table.find(database_connection, query_string, callback)

This function is not too different from doing a query directly on a
database connection.  The only extra thing it does is to turn the
result from a list of simple hash objects to a list of Row objects of
the corresponding table's "rowClass".

__Example__
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype.findAll"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>findAll (conn, cb)](#apidoc.element.node-mysql.Table.prototype.findAll)
- description and source-code
```javascript
findAll = function (conn, cb) {
    this.find(conn, this.baseQuery(), cb);
}
```
- example usage
```shell
...
'''

In this example, two threads are executed in parallel.  The thread of
setting value "bar1" will be block by the thread of setting value
"foo1".

<a name="table-findAll"/>
### table.findAll(database_connection, callback)

This finds all the rows in a table.

<a name="table-baseQuery"/>
### table.baseQuery(query_string, variable_bindings)

This is a short-hand for:
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype.findById"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>findById (conn, id, cb)](#apidoc.element.node-mysql.Table.prototype.findById)
- description and source-code
```javascript
findById = function (conn, id, cb) {
    var me = this;

    cps.seq([
        function(_, cb) {
            me.find(conn, me.baseQuery('where ' + me.getIdFieldName() + ' = ? ', [id]), cb);
        },
        function(res) {
            cb(null, res[0])
        }
    ], cb);
}
```
- example usage
```shell
...
        cb();
    }
], cb);
}, cb);
'''

<a name="table-findById"/>
### table.findById(database_connection, row_id, callback)

This is simply a short-hand for:

'''javascript
cps.seq([
function(_, cb) {
    table.find(
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype.findFirst"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>findFirst (conn, q, cb)](#apidoc.element.node-mysql.Table.prototype.findFirst)
- description and source-code
```javascript
findFirst = function (conn, q, cb) {
    var me = this;

    cps.seq([
        function(_, cb) {
            me.find(conn, q, cb);
        },
        function(res, cb) {
            cb(null, res[0]);
        }
    ], cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mysql.Table.prototype.getCreatedFieldName"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>getCreatedFieldName ()](#apidoc.element.node-mysql.Table.prototype.getCreatedFieldName)
- description and source-code
```javascript
getCreatedFieldName = function () {
    return this._createdFieldName;
}
```
- example usage
```shell
...
    return this._updatedFieldName;
},

_hasUpdatableField: function(field) {
    if (field == this.getIdFieldName()) {
        return false;
    }
    if (field == this.getCreatedFieldName()) {
        return false;
    }
    var schema = this._db._schema[this.getName()];
    return $U.contains(schema, field);
},

_refineDto: function(dto, autoId) {
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype.getIdFieldName"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>getIdFieldName ()](#apidoc.element.node-mysql.Table.prototype.getIdFieldName)
- description and source-code
```javascript
getIdFieldName = function () {
    return this._idFieldName;
}
```
- example usage
```shell
...
    var Row  = Class({
_init: function(data, cfg) {
    this._table = cfg.table;
    this._data = data;
},

getId: function() {
    return this._data[this._table.getIdFieldName()];
},

_getVersion: function() {
    return this._data[this._table.getVersionFieldName()];
},

_nextVersion: function() {
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype.getName"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>getName ()](#apidoc.element.node-mysql.Table.prototype.getName)
- description and source-code
```javascript
getName = function () {
    return this._name;
}
```
- example usage
```shell
...
        _update: function(conn, dto, conditions, cb) {
var me = this;

// dto[this._table.getUpdatedFieldName()] = new Date();
dto = this._refineDtoForUpdate(dto);

var l = [
    ' update ', this._table.getName(), ' set '
];

var first = true;
for (var k in dto) {
    var v = dto[k];
    if (first) {
        first = false;
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype.getUpdatedFieldName"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>getUpdatedFieldName ()](#apidoc.element.node-mysql.Table.prototype.getUpdatedFieldName)
- description and source-code
```javascript
getUpdatedFieldName = function () {
    return this._updatedFieldName;
}
```
- example usage
```shell
...
    for (var k in dto) {
        if (this._table._hasUpdatableField(k)) {
            res[k] = dto[k];
        }
    }

    var d = new Date();
    res[this._table.getUpdatedFieldName()] = d;

    return res;
},

updateWithoutOptimisticLock: function(conn, dto, cb) {
    this._update(conn, dto, null, cb);
},
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype.getVersionFieldName"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>getVersionFieldName ()](#apidoc.element.node-mysql.Table.prototype.getVersionFieldName)
- description and source-code
```javascript
getVersionFieldName = function () {
    return this._versionFieldName;
}
```
- example usage
```shell
...
},

getId: function() {
    return this._data[this._table.getIdFieldName()];
},

_getVersion: function() {
    return this._data[this._table.getVersionFieldName()];
},

_nextVersion: function() {
    return this._data[this._table.getVersionFieldName()] + 1;
},

_updateLocalData: function(dto) {
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype.linkedBy"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>linkedBy (cfg)](#apidoc.element.node-mysql.Table.prototype.linkedBy)
- description and source-code
```javascript
linkedBy = function (cfg) {
    this._linkedByMap[cfg.name] = {
        table: cfg.table,
        key: cfg.key
    };
    return this;
}
```
- example usage
```shell
...
idFieldName: 'order_id',
Row: {
    getFirstOrderItem: function(conn, cb) {
        var me = this;

        cps.seq([
            function(_, cb) {
                me.linkedBy(conn, 'items', cb);
            },
            function(items, cb) {
                cb(null, items[0]);
            }
        ], cb);
    }
},
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype.linksTo"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>linksTo (cfg)](#apidoc.element.node-mysql.Table.prototype.linksTo)
- description and source-code
```javascript
linksTo = function (cfg) {
    this._linksToMap[cfg.name] = {
        table: cfg.table,
        key: cfg.key
    };
    return this;
}
```
- example usage
```shell
...
}
})
.linkedBy({
    name: 'items',
    key: 'order_id',
    table: 'order_items'
})
.linksTo({
    name: 'user',
    key: 'user_id',
    table: 'users'
})
.linksTo({
    name: 'coupon',
    key: 'coupon_id',
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype.lockById"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>lockById (conn, id, cb)](#apidoc.element.node-mysql.Table.prototype.lockById)
- description and source-code
```javascript
lockById = function (conn, id, cb) {
    var me = this;

    cps.seq([
        function(_, cb) {
            me.find(conn, me.baseQuery('where ' + me.getIdFieldName() + ' = ? for update', [id]), cb);
        },
        function(res) {
            cb(null, res[0])
        }
    ], cb);
}
```
- example usage
```shell
...
], cb);
'''

It finds a row in a table by its primary ID and returns a single row
object of the table's corresponding rowClass.

<a name="table-lockById"/>
### table.lockById(database_connection, row_id, callback)

This function does the same thing as findById and additionally, it
locks the corresponding row for an atomic update.  lockById can ONLY
be used in a transaction context.  Without a transaction context, it
behaves the same as findById.  Once a row is locked in one
transaction, attempts of locking the same row in other transactions
will hang until the current transaction either commits or rolls back,
...
```

#### <a name="apidoc.element.node-mysql.Table.prototype.relatesTo"></a>[function <span class="apidocSignatureSpan">node-mysql.Table.prototype.</span>relatesTo (cfg)](#apidoc.element.node-mysql.Table.prototype.relatesTo)
- description and source-code
```javascript
relatesTo = function (cfg) {
    this._relatesToMap[cfg.name] = {
        table: cfg.table,
        through: cfg.through,
        leftKey: cfg.leftKey,
        rightKey: cfg.rightKey
    };
    return this;
}
```
- example usage
```shell
...

Once a "linkedBy" is set up on a table, a row object corresponding to
this table can call the "linkedBy" method to pull more (associated)
data into the row.  See examples [here](#row-linkedBy).

<a name="table-relatesTo"/>

### table.relatesTo(config)

The config object has the following schema:

'''json
{
"name": {
    "type": "String",
...
```



# <a name="apidoc.module.node-mysql.db"></a>[module node-mysql.db](#apidoc.module.node-mysql.db)

#### <a name="apidoc.element.node-mysql.db.db"></a>[function <span class="apidocSignatureSpan">node-mysql.</span>db ()](#apidoc.element.node-mysql.db.db)
- description and source-code
```javascript
db = function () {
    this._init.apply(this, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mysql.db.format"></a>[function <span class="apidocSignatureSpan">node-mysql.db.</span>format (str, bindings)](#apidoc.element.node-mysql.db.format)
- description and source-code
```javascript
format = function (str, bindings) {
    var l = str.split('?')

    if (l.length - 1 != bindings.length) {
        throw new Error('sql string format error');
    }

    var res = [];

    for (var i = 0; i < bindings.length; i++) {
        res.push(l[i]);
        res.push(mysql.escape(bindings[i]));
    }

    res.push(l[l.length - 1]);

    return res.join(' ');
}
```
- example usage
```shell
...
        }
    ], cb);
}, cb);
'''


<a name="DB-format" />
### DB.format(query_string, variable_bindings)

This is a wrapper of the query string formatting functionality
provided by the mysql package.  Note that this is a global static
method defined on the class DB.  It is NOT an instance method defined
a a DB instance db.

__Example__
...
```



# <a name="apidoc.module.node-mysql.db.prototype"></a>[module node-mysql.db.prototype](#apidoc.module.node-mysql.db.prototype)

#### <a name="apidoc.element.node-mysql.db.prototype._buildCfg"></a>[function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>_buildCfg (cfg, override)](#apidoc.element.node-mysql.db.prototype._buildCfg)
- description and source-code
```javascript
_buildCfg = function (cfg, override) {
    var res = {};

    for (var k in cfg) {
        res[k] = cfg[k];
    }

    $U.extend(res, override);
    return res;
}
```
- example usage
```shell
...
delete cfg['useCursor'];

this._cfg = cfg;
// console.log(this._cfg);
this._pool = mysql.createPool(this._cfg);

if (transactionOverride) {
    this._transactionCfg = this._buildCfg(cfg, transactionOverride);
    // console.log('transactionCfg:', this._transactionCfg);
    this._transactionPool = mysql.createPool(this._transactionCfg);
}

if (cursorOverride) {
    this._cursorCfg = this._buildCfg(cfg, cursorOverride);
    // console.log('cursorCfg:', this._cursorCfg);
...
```

#### <a name="apidoc.element.node-mysql.db.prototype._connect"></a>[function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>_connect (pool, proc, cb)](#apidoc.element.node-mysql.db.prototype._connect)
- description and source-code
```javascript
_connect = function (pool, proc, cb) {
    var me = this;
    var conn;
    cps.seq([
        function(_, cb) {
            pool.getConnection(cb);
        },
        function(res, cb) {
            conn = res;
            cps.rescue({
                'try': function(cb) {
                    proc(conn, cb);
                },
                'finally': function(cb) {
                    // console.log('release connection');
                    conn.release();
                    cb();
                }
            }, cb);
        }
    ], cb);
}
```
- example usage
```shell
...
    var me = this;

    cps.seq([
        function(_, cb) {
            me._prepare(cb);
        },
        function(_, cb) {
            me._connect(me._pool, proc, cb);
        }
    ], cb);
},

_prepare: function(cb) {
    if (this._prepared) {
        return cb();
...
```

#### <a name="apidoc.element.node-mysql.db.prototype._enterTransaction"></a>[function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>_enterTransaction (conn)](#apidoc.element.node-mysql.db.prototype._enterTransaction)
- description and source-code
```javascript
_enterTransaction = function (conn) {
    conn.__transaction__ = true;
}
```
- example usage
```shell
...
/*
function(_, cb) {
    me._getTxnConnection(cb);
},
*/
function(_, cb) {
    me._connect(me._transactionPool, function(conn, cb) {
        me._enterTransaction(conn);
        txnConn = conn;
        cps.rescue({
            'try': function(cb) {
                cps.seq([
                    function(_, cb) {
                        // console.log('start transaction');
                        txnConn.query('START TRANSACTION', cb);
...
```

#### <a name="apidoc.element.node-mysql.db.prototype._init"></a>[function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>_init (cfg)](#apidoc.element.node-mysql.db.prototype._init)
- description and source-code
```javascript
_init = function (cfg) {
    var transactionOverride = cfg['useTransaction'];
    delete cfg['useTransaction'];

    var cursorOverride = cfg['useCursor'];
    delete cfg['useCursor'];

    this._cfg = cfg;
    // console.log(this._cfg);
    this._pool = mysql.createPool(this._cfg);

    if (transactionOverride) {
        this._transactionCfg = this._buildCfg(cfg, transactionOverride);
        // console.log('transactionCfg:', this._transactionCfg);
        this._transactionPool = mysql.createPool(this._transactionCfg);
    }

    if (cursorOverride) {
        this._cursorCfg = this._buildCfg(cfg, cursorOverride);
        // console.log('cursorCfg:', this._cursorCfg);
        this._cursorPool = mysql.createPool(this._cursorCfg);
    }

    this._schema = {};
    this._prepared = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mysql.db.prototype._isTxnConnection"></a>[function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>_isTxnConnection (conn)](#apidoc.element.node-mysql.db.prototype._isTxnConnection)
- description and source-code
```javascript
_isTxnConnection = function (conn) {
    return conn != null && conn.__transaction__;
}
```
- example usage
```shell
...
    cb(new Error('transaction-not-setup-error'));
    return;
}

var txnConn;
var commitRes;

if (me._isTxnConnection(conn)) {
    proc(conn, cb);
} else {
    cps.seq([
        function(_, cb) {
            me._prepare(cb);
        },
        /*
...
```

#### <a name="apidoc.element.node-mysql.db.prototype._leaveTransaction"></a>[function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>_leaveTransaction (conn)](#apidoc.element.node-mysql.db.prototype._leaveTransaction)
- description and source-code
```javascript
_leaveTransaction = function (conn) {
    conn.__transaction__ = false;
}
```
- example usage
```shell
...
                                }, cb);
                            }
                        ], cb);
                    },
                    'finally': function(cb) {
                        // console.log('txn connection release');
                        // txnConn.release();
                        me._leaveTransaction(txnConn);
                        cb();
                    }
                }, cb);
            }, cb);
        }
    ], cb);
}
...
```

#### <a name="apidoc.element.node-mysql.db.prototype._prepare"></a>[function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>_prepare (cb)](#apidoc.element.node-mysql.db.prototype._prepare)
- description and source-code
```javascript
_prepare = function (cb) {
    if (this._prepared) {
        return cb();
    }

    // console.log('call prepare');
    var me = this;
    var conn;

    this._connect(me._pool, function(conn, cb) {
        cps.seq([
            function(res, cb) {
                conn.query('show tables', cb);
            },
            function(tables, cb) {
                cps.peach(tables, function(table, cb) {
                    var tableName = getValue(table);
                    cps.seq([
                        function(_, cb) {
                            conn.query('desc ' + tableName, cb);
                        },
                        function(columns, cb) {
                            me._schema[tableName] = $U.map(columns, function(column) {
                                return column['Field'];
                            });
                            me._prepared = true;
                            cb();
                        }
                    ], cb);
                }, cb);
            }
        ], cb);
    }, cb);
}
```
- example usage
```shell
...
},

connect: function(proc, cb) {
    var me = this;

    cps.seq([
        function(_, cb) {
            me._prepare(cb);
        },
        function(_, cb) {
            me._connect(me._pool, proc, cb);
        }
    ], cb);
},
...
```

#### <a name="apidoc.element.node-mysql.db.prototype.connect"></a>[function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>connect (proc, cb)](#apidoc.element.node-mysql.db.prototype.connect)
- description and source-code
```javascript
connect = function (proc, cb) {
    var me = this;

    cps.seq([
        function(_, cb) {
            me._prepare(cb);
        },
        function(_, cb) {
            me._connect(me._pool, proc, cb);
        }
    ], cb);
}
```
- example usage
```shell
...
    database : 'prod_clone',
    connectionLimit: 1
}
'''


<a name="db-connect">
### db.connect(procedure, callback)

The procedure is a function of the type:

'''javascript
function(connection, callback) {
    // work with the database connection
}
...
```

#### <a name="apidoc.element.node-mysql.db.prototype.cursor"></a>[function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>cursor (q, proc, _cb)](#apidoc.element.node-mysql.db.prototype.cursor)
- description and source-code
```javascript
cursor = function (q, proc, _cb) {
    var me = this;

    if (!me._cursorPool) {
        _cb(new Error('cursor-not-setup-error'));
        return;
    }

    var returned = false;

    var cb = function(err, res) {
        if (!returned) {
            returned = true;
            _cb(err, res);
        } else {
        }
    }

    var breakCB =  cb;
    this._cursorPool.getConnection(function(err, conn) {
        var query = conn.query(q);
        query
            .on('error', function(err) {
                // console.log('cursor error');
                conn.release();
                cb(new Error(err));
            })
            .on('result', function(res) {
                // console.log('cursor result');
                conn.pause();

                var cb = function(err, res) {
                    if (err) {
                        conn.release();
                        breakCB(err);
                    } else {
                        conn.resume();
                    }
                };

                cps.seq([
                    function(_, cb) {
                        // console.log('call row processor');
                        proc(res, cb);
                    }
                ], cb);
            })
            .on('end', function() {
                // console.log('cursor end');
                conn.release();
                cb();
            })
        ;
    });
}
```
- example usage
```shell
...
          ], cb);
      // }, cb);
  }, cb);
};
'''

<a name="db-cursor"/>
### db.cursor(query_string, procedure, callback)

This API can be used to cursor thought the (potentially very long list
of) results of a query.  The procedure parameter is the operation to
be applied to each row in the results of the query.  Please note the following:

* db.cursor will create a separate db connection for cursoring
purpose.  That is why this API does not take a db_connection in the
...
```

#### <a name="apidoc.element.node-mysql.db.prototype.end"></a>[function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>end ()](#apidoc.element.node-mysql.db.prototype.end)
- description and source-code
```javascript
end = function () {
    this._pool.end();
    if (this._transactionPool) {
        this._transactionPool.end();
    }
    if (this._cursorPool) {
        this._cursorPool.end();
    }
}
```
- example usage
```shell
...
};
'''




<a name="db-end" />
### db.end();

This function destructs the db object.

<a name="db-add"/>

### db.add(config);
...
```

#### <a name="apidoc.element.node-mysql.db.prototype.getConnection"></a>[function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>getConnection (cb)](#apidoc.element.node-mysql.db.prototype.getConnection)
- description and source-code
```javascript
getConnection = function (cb) {
    var me = this;

    cps.seq([
        function(_, cb) {
            me._prepare(cb);
        },
        function(_, cb) {
            me._pool.getConnection(cb);
        }
    ], cb);
}
```
- example usage
```shell
...
},

_connect: function(pool, proc, cb) {
    var me = this;
    var conn;
    cps.seq([
        function(_, cb) {
            pool.getConnection(cb);
        },
        function(res, cb) {
            conn = res;
            cps.rescue({
                'try': function(cb) {
                    proc(conn, cb);
                },
...
```

#### <a name="apidoc.element.node-mysql.db.prototype.transaction"></a>[function <span class="apidocSignatureSpan">node-mysql.db.prototype.</span>transaction (conn, proc, cb)](#apidoc.element.node-mysql.db.prototype.transaction)
- description and source-code
```javascript
transaction = function (conn, proc, cb) {
    var me = this;

    if (!me._transactionPool) {
        cb(new Error('transaction-not-setup-error'));
        return;
    }

    var txnConn;
    var commitRes;

    if (me._isTxnConnection(conn)) {
        proc(conn, cb);
    } else {
        cps.seq([
            function(_, cb) {
                me._prepare(cb);
            },
<span class="apidocCodeCommentSpan">            /*
            function(_, cb) {
                me._getTxnConnection(cb);
            },
            */
</span>            function(_, cb) {
                me._connect(me._transactionPool, function(conn, cb) {
                    me._enterTransaction(conn);
                    txnConn = conn;
                    cps.rescue({
                        'try': function(cb) {
                            cps.seq([
                                function(_, cb) {
                                    // console.log('start transaction');
                                    txnConn.query('START TRANSACTION', cb);
                                },
                                function(_, cb) {
                                    cps.rescue({
                                        'try': function(cb) {
                                            cps.seq([
                                                function(_, cb) {
                                                    proc(txnConn, cb);
                                                },
                                                function(res, cb) {
                                                    commitRes = res;
                                                    // console.log('committing');
                                                    txnConn.query('COMMIT', cb);
                                                },
                                                function(_, cb) {
                                                    // console.log('committed');
                                                    cb(null, commitRes);
                                                }
                                            ], cb);
                                        },
                                        'catch': function(err, cb) {
                                            cps.seq([
                                                function(_, cb) {
                                                    // console.log('rolling back ...');
                                                    txnConn.query('ROLLBACK', cb);
                                                },
                                                function(_, cb) {
                                                    // console.log('rolled back');
                                                    throw(err);
                                                }
                                            ], cb);
                                        }
                                    }, cb);
                                }
                            ], cb);
                        },
                        'finally': function(cb) {
                            // console.log('txn connection release');
                            // txnConn.release();
                            me._leaveTransaction(txnConn);
                            cb();
                        }
                    }, cb);
                }, cb);
            }
        ], cb);
    }
}
```
- example usage
```shell
...
            }
        ], cb);
    }, cb);
};
'''

<a name="db-transaction"/>
### db.transaction(db_connection, procedure, callback)

The procedure is a function of the type:

'''javascript
function(connection, callback) {
    // work with the database connection
}
...
```



# <a name="apidoc.module.node-mysql.model"></a>[module node-mysql.model](#apidoc.module.node-mysql.model)

#### <a name="apidoc.element.node-mysql.model.Row"></a>[function <span class="apidocSignatureSpan">node-mysql.model.</span>Row ()](#apidoc.element.node-mysql.model.Row)
- description and source-code
```javascript
Row = function () {
    this._init.apply(this, arguments);
}
```
- example usage
```shell
...
var q = 'select * from users';

db.cursor(q, function(row, cb) {
    cps.rescur({
        'try': function() {
            cps.seq([
                function(_, cb) {
                    var user = new User.Row(row);
                    user.update(conn, {active: 1}, cb);
                },
                function(res, cb) {
                    console.log(res);
                    cb();
                }
            ], cb);
...
```

#### <a name="apidoc.element.node-mysql.model.Table"></a>[function <span class="apidocSignatureSpan">node-mysql.model.</span>Table ()](#apidoc.element.node-mysql.model.Table)
- description and source-code
```javascript
Table = function () {
    this._init.apply(this, arguments);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
