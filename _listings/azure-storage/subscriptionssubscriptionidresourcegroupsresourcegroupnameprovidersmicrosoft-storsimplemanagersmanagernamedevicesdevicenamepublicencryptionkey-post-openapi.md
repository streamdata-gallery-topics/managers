---
swagger: "2.0"
x-collection-name: Azure Storage
x-complete: 0
info:
  title: Azure Storage API Managers Get Device Public Encryption Key
  version: 1.0.0
  description: Returns the public encryption key of the device.
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /subscriptions/{subscriptionId}/providers/Microsoft.StorSimple/managers:
    get:
      summary: Managers List
      description: Retrieves all the managers in a subscription.
      operationId: Managers_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-storsimplemanagers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Managers
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorSimple/managers/{managerName}:
    get:
      summary: Managers Get
      description: Returns the properties of the specified manager name.
      operationId: Managers_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagername-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Managers
    put:
      summary: Managers Create Or Update
      description: Creates or updates the manager.
      operationId: Managers_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagername-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The manager
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Managers
    delete:
      summary: Managers Delete
      description: Deletes the manager.
      operationId: Managers_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagername-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Managers
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.StorSimple/managers/{managerName}/devices/{deviceName}/publicEncryptionKey
  : post:
      summary: Managers Get Device Public Encryption Key
      description: Returns the public encryption key of the device.
      operationId: Managers_GetDevicePublicEncryptionKey
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-storsimplemanagersmanagernamedevicesdevicenamepublicencryptionkey-post
      parameters:
      - in: path
        name: deviceName
        description: The device name
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Managers
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---