.. Copyright 2017 FUJITSU LIMITED

.. _mySoftwareRestriction-update:

mySoftwareRestriction_update
----------------------------

.. function:: PUT /users/{uid}/mysoftware/{msid}/restrictions/{brid}

.. sidebar:: Summary

	* Method: ``PUT``
	* Response Code: ``200``
	* Response Formats: ``application/xml`` ``application/json``
	* Since: ``UForge 3.6``

Updates the bundle restriction for a software component. 

This only updates the list of distributions for which the software component is designed for

Security Summary
~~~~~~~~~~~~~~~~

* Requires Authentication: ``true``
* Entitlements Required: ``software_upload``

URI Parameters
~~~~~~~~~~~~~~

* ``uid`` (required): the id of the :ref:`user-object`
* ``msid`` (required): the id of the :ref:`mySoftware-object`
* ``brid`` (required): the id of the :ref:`bundlerestriction-object`

HTTP Request Body Parameters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A :ref:`bundleRestriction-object` object

Example Request
~~~~~~~~~~~~~~~

.. code-block:: bash

	curl "https://uforge.example.com/api/users/{uid}/mysoftware/{msid}/restrictions/{brid}" -X PUT \
	-u USER_LOGIN:PASSWORD -H "Accept: application/xml" --data-binary "@representation.xml"

Example of representation.xml content (the request body):

.. code-block:: xml



.. seealso::

	 * :ref:`mySoftware-object`
	 * :ref:`mySoftwareArtifact-add`
	 * :ref:`mySoftwareArtifact-addChild`
	 * :ref:`mySoftwareArtifact-addOrRemoveFileFromCache`
	 * :ref:`mySoftwareArtifact-createFromRemoteServer`
	 * :ref:`mySoftwareArtifact-delete`
	 * :ref:`mySoftwareArtifact-deleteAll`
	 * :ref:`mySoftwareArtifact-download`
	 * :ref:`mySoftwareArtifact-downloadFile`
	 * :ref:`mySoftwareArtifact-get`
	 * :ref:`mySoftwareArtifact-getAll`
	 * :ref:`mySoftwareArtifact-updateAll`
	 * :ref:`mySoftwareArtifact-upload`
	 * :ref:`mySoftwareExportStatus-get`
	 * :ref:`mySoftwareExport-delete`
	 * :ref:`mySoftwareExport-download`
	 * :ref:`mySoftwareLicense-delete`
	 * :ref:`mySoftwareLicense-download`
	 * :ref:`mySoftwareLicense-upload`
	 * :ref:`mySoftwareLicense-uploadFile`
	 * :ref:`mySoftwareLogo-delete`
	 * :ref:`mySoftwareLogo-download`
	 * :ref:`mySoftwareLogo-downloadFile`
	 * :ref:`mySoftwareLogo-upload`
	 * :ref:`mySoftwareOs-getAll`
	 * :ref:`mySoftwareRestrictionOs-getAll`
	 * :ref:`mySoftwareRestrictionOs-getAll`
	 * :ref:`mySoftwareRestriction-add`
	 * :ref:`mySoftwareRestriction-delete`
	 * :ref:`mySoftwareRestriction-delete`
	 * :ref:`mySoftwareRestriction-deleteAll`
	 * :ref:`mySoftwareRestriction-deleteAll`
	 * :ref:`mySoftwareRestriction-get`
	 * :ref:`mySoftwareRestriction-getAll`
	 * :ref:`mySoftwareRestriction-update`
	 * :ref:`mySoftwareUsage-getAll`
	 * :ref:`mySoftware-clone`
	 * :ref:`mySoftware-create`
	 * :ref:`mySoftware-delete`
	 * :ref:`mySoftware-export`
	 * :ref:`mySoftware-get`
	 * :ref:`mySoftware-getAll`
	 * :ref:`mySoftware-update`
	 * :ref:`softwareBundleImport-get`
	 * :ref:`softwareartifact-object`
	 * :ref:`softwarebundleImportStatus-get`
	 * :ref:`softwarebundleImport-upload`
	 * :ref:`softwarebundle-import`