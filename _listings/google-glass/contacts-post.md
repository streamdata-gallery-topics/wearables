---
swagger: "2.0"
info:
  title: Google Mirror
  description: Interacts with Glass users via the timeline.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /mirror/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /contacts:
    post:
      summary: Insert Contact
      description: Inserts a new contact
      operationId: mirror.contacts.insert
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - contact
definitions:
  Account:
    properties:
      authTokens:
        description: This is a default description.
        type: parameters
      features:
        description: This is a default description.
        type: parameters
      password:
        description: This is a default description.
        type: parameters
      userData:
        description: This is a default description.
        type: parameters
  Attachment:
    properties:
      contentType:
        description: This is a default description.
        type: parameters
      contentUrl:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      isProcessingContent:
        description: This is a default description.
        type: parameters
  AttachmentsListResponse:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  AuthToken:
    properties:
      authToken:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  Command:
    properties:
      type:
        description: This is a default description.
        type: parameters
  Contact:
    properties:
      acceptCommands:
        description: This is a default description.
        type: parameters
      acceptTypes:
        description: This is a default description.
        type: parameters
      displayName:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      imageUrls:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      phoneNumber:
        description: This is a default description.
        type: parameters
      priority:
        description: This is a default description.
        type: parameters
      sharingFeatures:
        description: This is a default description.
        type: parameters
      source:
        description: This is a default description.
        type: parameters
  ContactsListResponse:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  Location:
    properties:
      accuracy:
        description: This is a default description.
        type: parameters
      address:
        description: This is a default description.
        type: parameters
      displayName:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      latitude:
        description: This is a default description.
        type: parameters
      longitude:
        description: This is a default description.
        type: parameters
      timestamp:
        description: This is a default description.
        type: parameters
  LocationsListResponse:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  MenuItem:
    properties:
      action:
        description: This is a default description.
        type: parameters
      contextual_command:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      payload:
        description: This is a default description.
        type: parameters
      removeWhenSelected:
        description: This is a default description.
        type: parameters
      values:
        description: This is a default description.
        type: parameters
  MenuValue:
    properties:
      displayName:
        description: This is a default description.
        type: parameters
      iconUrl:
        description: This is a default description.
        type: parameters
      state:
        description: This is a default description.
        type: parameters
  Notification:
    properties:
      collection:
        description: This is a default description.
        type: parameters
      itemId:
        description: This is a default description.
        type: parameters
      operation:
        description: This is a default description.
        type: parameters
      userActions:
        description: This is a default description.
        type: parameters
      userToken:
        description: This is a default description.
        type: parameters
      verifyToken:
        description: This is a default description.
        type: parameters
  NotificationConfig:
    properties:
      deliveryTime:
        description: This is a default description.
        type: parameters
      level:
        description: This is a default description.
        type: parameters
  Setting:
    properties:
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
  Subscription:
    properties:
      callbackUrl:
        description: This is a default description.
        type: parameters
      collection:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      operation:
        description: This is a default description.
        type: parameters
      updated:
        description: This is a default description.
        type: parameters
      userToken:
        description: This is a default description.
        type: parameters
      verifyToken:
        description: This is a default description.
        type: parameters
  SubscriptionsListResponse:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
  TimelineItem:
    properties:
      attachments:
        description: This is a default description.
        type: parameters
      bundleId:
        description: This is a default description.
        type: parameters
      canonicalUrl:
        description: This is a default description.
        type: parameters
      created:
        description: This is a default description.
        type: parameters
      displayTime:
        description: This is a default description.
        type: parameters
      etag:
        description: This is a default description.
        type: parameters
      html:
        description: This is a default description.
        type: parameters
      id:
        description: This is a default description.
        type: parameters
      inReplyTo:
        description: This is a default description.
        type: parameters
      isBundleCover:
        description: This is a default description.
        type: parameters
  TimelineListResponse:
    properties:
      items:
        description: This is a default description.
        type: parameters
      kind:
        description: This is a default description.
        type: parameters
      nextPageToken:
        description: This is a default description.
        type: parameters
  UserAction:
    properties:
      payload:
        description: This is a default description.
        type: parameters
      type:
        description: This is a default description.
        type: parameters
  UserData:
    properties:
      key:
        description: This is a default description.
        type: parameters
      value:
        description: This is a default description.
        type: parameters
x-collection-name: Google Glass
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