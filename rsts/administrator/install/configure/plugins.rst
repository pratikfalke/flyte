.. _plugins-config:

#########################
Plugin Configuration
#########################

.. _plugins-config-enable:

Controlling the plugins available
=================================

+---------------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Config Val                                         |Type            |Description                                                                                                                                                                                               |
+---------------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|plugins.enabled-plugins                            |strings         |List of enabled plugins, default value is to enable all plugins. (default [*])                                                                                                                            |
+---------------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. _plugins-config-log-links:

Controlling log-links for user containers
=========================================

+---------------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|Config Val                                         |Type            |Description                                                                                                                                                                                               |
+---------------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|plugins.logs.cloudwatch-enabled                    |Bool            |Cloudwatch Logging                                                                                                                                                                                        |
+---------------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|plugins.logs.cloudwatch-log-group                  |string          |Log group to which streams are associated.                                                                                                                                                                |
+---------------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|plugins.logs.cloudwatch-region                     |string          |AWS region in which Cloudwatch logs are stored.                                                                                                                                                           |
+---------------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|plugins.logs.kubernetes-enabled                    |Bool            |Kubernetes Logging                                                                                                                                                                                        |
+---------------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
|plugins.logs.kubernetes-url                        |string          |Console URL for Kubernetes logs                                                                                                                                                                           |
+---------------------------------------------------+----------------+----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

.. _plugins-config-k8s-defaults:

Default values to provide kubernetes container executions
=========================================================


.. _plugins-config-per-plugin:

Individual plugins configuration
================================
Refer to plugin documentation for understanding the configuration alternatives


.. _plugins-config-example:

Example Configuration
=====================

Top level Plugin configuration example
--------------------------------------

.. literalinclude:: ../../../../kustomize/overlays/sandbox/propeller/plugins/config.yaml

Individual plugin configuration example
---------------------------------------

Spark

.. literalinclude:: ../../../../kustomize/overlays/sandbox/propeller/plugins/spark/config.yaml

Qubole

.. literalinclude:: ../../../../kustomize/overlays/sandbox/propeller/plugins/qubole/config.yaml
