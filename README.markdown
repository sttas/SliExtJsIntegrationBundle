# This bundle is not longer maintained, only critical bugfixes will be applied, please use [SliDoctrineArrayQueryBuilderBundle](https://github.com/sergeil/SliDoctrineArrayQueryBuilderBundle) and [SliDoctrineEntityDataMapperBundle](https://github.com/sergeil/SliDoctrineEntityDataMapperBundle) instead.

The bundle will contain some utility classes that prove useful when you use ExtJs library on the client-side.

What's inside
=============
For now, there's not much yet:

 * QueryBuilder\ExtjsQueryBuilder -- Builds proper Doctrine queries for your ``Ext.data.Store`` on client-side. Makes it possible
                                to easily leverage 'remoteFilter', 'remoteSort' as well as pagination. Also, the class is smart
                                enough to build proper queries when you need to sort(ORDER BY) by an associated entity
 * DataMapping\EntityDataMapperService -- Maps data coming from client-side onto your entities

Please read inline phpDoc for more information how to use classes

Installation
============
1. Add the bundle to your composer.json:
   ```
   {
       "require": {
           "sergeil/extjsintegration-bundle": "~1.0"
       }
   }
   ```

2. Add bundles to your ``/app/AppKernel``:
    ```
    new Sli\ExtJsIntegrationBundle\SliExtJsIntegrationBundle(),
    new Sli\AuxBundle\SliAuxBundle()
    ```