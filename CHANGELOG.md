CHANGELOG
=========

0.10.1
-------

* Improve leo_hex performances
    * "binary_to_hex" function
    * Related libs:
        * leo_gateway
        * leo_object_storage
        * leo_redundant_manager
    * By this correspondence, LeoFS's performance improved 20% up.
* Improve leo_manager
    * Format of output from manager-console
        * Commands:
            * "status"
            * "whereis"
* Improve performance of "storage-stats" in manager-console
* Fix bugs
    * A handling error in S3-libs


0.10.0
-------

* Improve S3-API's compatibility
    * Add S3-authentication
    * Add S3-bucket
* Add S3-related command in LeoFS's manager
    * "s3-gen-key" : Generate a S3 key pair(AccessKeyID and SecretAccessKey)
    * "s3-set-endpoint" : Register a new S3 Endpoint
    * "s3-delete-endpoint" : Delete a S3 Endpoint
    * "s3-get-endpoints" : Retrieve all of S3 Endpoints registered
    * "s3-get-buckets" : Retrieve all of Buckets registered
* Improve order of system launch
    * Remove "attach command" in manager - After Storage launched, the node's state is automatically changed to "attached"
* Improve rebalance-function's performance which is about 5 times compare with v0.9.1
* Improve compact-function. Restrain storage's load when compact objects.
* Fix bugs
    * Deletion of Zero bytes in Storage
    * Behavior after the restart of Manager
    * Re-register procs into the Manager's monitor


0.9.1
-----

* Remove "apps" directory in leofs - Modified "reltool.config"
* Fix 'shadow vars'
* Remove ZMQ log-appender and AMQP log-appender for leo_logger, They will be provided LeoFS's sub projects.
* Improve - In order to be able to extend "LeoFS's Object Container's file format".


0.9.0
-----

* Initial release
