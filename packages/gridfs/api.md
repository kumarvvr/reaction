## cfs-gridfs Public API ##

GridFS storage adapter for CollectionFS

_API documentation automatically generated by [docmeteor](https://github.com/raix/docmeteor)._

-

### <a name="FS.Store.GridFS"></a>new *fsStore*.GridFS(name, options)&nbsp;&nbsp;<sub><i>Server</i></sub> ###

*This method __GridFS__ is defined in `FS.Store`*

__Arguments__

* __name__ *{String}*  

 The store name

* __options__ *{Object}*  
    * __beforeSave__ *{Function}*  (Optional)

     Function to run before saving a file from the server. The context of the function will be the `FS.File` instance we're saving. The function may alter its properties.

    * __maxTries__ *{Number}*  (Optional, Default = 5)

     Max times to attempt saving a file


__Returns__  *{FS.StorageAdapter}*
An instance of FS.StorageAdapter.


Creates a GridFS store instance on the server. Inherits from FS.StorageAdapter
type.

> ```FS.Store.GridFS = function(name, options) { ...``` [gridfs.server.js:16](gridfs.server.js#L16)


-

### <a name="FS.Store.GridFS"></a>new *fsStore*.GridFS(name, options)&nbsp;&nbsp;<sub><i>Client</i></sub> ###

*This method __GridFS__ is defined in `FS.Store`*

__Arguments__

* __name__ *{String}*  

 The store name

* __options__ *{Object}*  
    * __beforeSave__ *{Function}*  (Optional)

     Function to run before saving a file from the client. The context of the function will be the `FS.File` instance we're saving. The function may alter its properties.

    * __maxTries__ *{Number}*  (Optional, Default = 5)

     Max times to attempt saving a file


__Returns__  *{undefined}*


Creates a GridFS store instance on the client, which is just a shell object
storing some info.

> ```FS.Store.GridFS = function(name, options) { ...``` [gridfs.client.js:13](gridfs.client.js#L13)


