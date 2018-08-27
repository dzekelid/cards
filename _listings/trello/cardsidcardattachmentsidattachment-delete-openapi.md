---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Delete Cards Attachments Attachment
  description: Delete cards attachments attachment.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /boards/{idBoard}/cards:
    get:
      summary: Get Boards Cards
      description: Get boards cards.
      operationId: getBoardsCardsByIdBoard
      x-api-path-slug: boardsidboardcards-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: attachments
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: query
        name: attachment_fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: query
        name: before
        description: A date, or null
      - in: query
        name: checkItemStates
        description: true or false
      - in: query
        name: checklists
        description: 'One of: all or none'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: filter
        description: 'One of: all, closed, none, open or visible'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: limit
        description: a number from 1 to 1000
      - in: query
        name: members
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: since
        description: A date, or null
      - in: query
        name: stickers
        description: true or false
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Cards
  /boards/{idBoard}/cards/{filter}:
    get:
      summary: Get Boards Cards Filter
      description: Get boards cards filter.
      operationId: getBoardsCardsByIdBoardByFilter
      x-api-path-slug: boardsidboardcardsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Cards
      - Filter
  /boards/{idBoard}/cards/{idCard}:
    get:
      summary: Get Boards Cards
      description: Get boards cards.
      operationId: getBoardsCardsByIdBoardByIdCard
      x-api-path-slug: boardsidboardcardsidcard-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: actions_display
        description: true or false
      - in: query
        name: actions_entities
        description: true or false
      - in: query
        name: actions_limit
        description: a number from 0 to 1000
      - in: query
        name: action_fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator
          or type'
      - in: query
        name: action_memberCreator_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: attachments
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: query
        name: attachment_fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: query
        name: checkItemStates
        description: true or false
      - in: query
        name: checkItemState_fields
        description: 'all or a comma-separated list of: idCheckItem or state'
      - in: query
        name: checklists
        description: 'One of: all or none'
      - in: query
        name: checklist_fields
        description: 'all or a comma-separated list of: idBoard, idCard, name or pos'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idCard
        description: idCard
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: labels
        description: true or false
      - in: query
        name: members
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Cards
  /boards/{idBoard}/members/{idMember}/cards:
    get:
      summary: Get Boards Members Cards
      description: Get boards members cards.
      operationId: getBoardsMembersCardsByIdBoardByIdMember
      x-api-path-slug: boardsidboardmembersidmembercards-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: attachments
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: query
        name: attachment_fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: query
        name: board
        description: true or false
      - in: query
        name: board_fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: query
        name: checkItemStates
        description: true or false
      - in: query
        name: checklists
        description: 'One of: all or none'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: filter
        description: 'One of: all, closed, none, open or visible'
      - in: path
        name: idBoard
        description: board_id
      - in: path
        name: idMember
        description: idMember
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: list
        description: true or false
      - in: query
        name: list_fields
        description: 'all or a comma-separated list of: closed, idBoard, name, pos
          or subscribed'
      - in: query
        name: members
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Members
      - Cards
  /cards:
    post:
      summary: Post Cards
      description: Post cards.
      operationId: addCards
      x-api-path-slug: cards-post
      parameters:
      - in: body
        name: body
        description: Attributes of Cards to be added
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
  /cards/{idCard}:
    delete:
      summary: Delete Cards
      description: Delete cards.
      operationId: deleteCardsByIdCard
      x-api-path-slug: cardsidcard-delete
      parameters:
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
    get:
      summary: Get Cards
      description: Get cards.
      operationId: getCardsByIdCard
      x-api-path-slug: cardsidcard-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: actions_display
        description: true or false
      - in: query
        name: actions_entities
        description: true or false
      - in: query
        name: actions_limit
        description: a number from 0 to 1000
      - in: query
        name: action_fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator
          or type'
      - in: query
        name: action_memberCreator_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: attachments
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: query
        name: attachment_fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: query
        name: board
        description: true or false
      - in: query
        name: board_fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: query
        name: checkItemStates
        description: true or false
      - in: query
        name: checkItemState_fields
        description: 'all or a comma-separated list of: idCheckItem or state'
      - in: query
        name: checklists
        description: 'One of: all or none'
      - in: query
        name: checklist_fields
        description: 'all or a comma-separated list of: idBoard, idCard, name or pos'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: list
        description: true or false
      - in: query
        name: list_fields
        description: 'all or a comma-separated list of: closed, idBoard, name, pos
          or subscribed'
      - in: query
        name: members
        description: true or false
      - in: query
        name: membersVoted
        description: true or false
      - in: query
        name: memberVoted_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: stickers
        description: true or false
      - in: query
        name: sticker_fields
        description: 'all or a comma-separated list of: image, imageScaled, imageUrl,
          left, rotate, top or zIndex'
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
    put:
      summary: Put Cards
      description: Put cards.
      operationId: updateCardsByIdCard
      x-api-path-slug: cardsidcard-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
  /cards/{idCard}/actions:
    get:
      summary: Get Cards Actions
      description: Get cards actions.
      operationId: getCardsActionsByIdCard
      x-api-path-slug: cardsidcardactions-get
      parameters:
      - in: query
        name: before
        description: A date, or null
      - in: query
        name: display
        description: true or false
      - in: query
        name: entities
        description: true or false
      - in: query
        name: fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator
          or type'
      - in: query
        name: filter
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: format
        description: 'One of: count, list or minimal'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: idModels
        description: Only return actions related to these model ids
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: limit
        description: a number from 0 to 1000
      - in: query
        name: member
        description: true or false
      - in: query
        name: memberCreator
        description: true or false
      - in: query
        name: memberCreator_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: page
        description: Page * limit must be less than 1000
      - in: query
        name: since
        description: A date, null or lastView
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Actions
  /cards/{idCard}/actions/comments:
    post:
      summary: Post Cards Actions Comments
      description: Post cards actions comments.
      operationId: addCardsActionsCommentsByIdCard
      x-api-path-slug: cardsidcardactionscomments-post
      parameters:
      - in: body
        name: body
        description: Attributes of Actions Comments to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Actions
      - Comments
  /cards/{idCard}/actions/{idAction}/comments:
    delete:
      summary: Delete Cards Actions Comments
      description: Delete cards actions comments.
      operationId: deleteCardsActionsCommentsByIdCardByIdAction
      x-api-path-slug: cardsidcardactionsidactioncomments-delete
      parameters:
      - in: path
        name: idAction
        description: idAction
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Actions
      - Comments
    put:
      summary: Put Cards Actions Comments
      description: Put cards actions comments.
      operationId: updateCardsActionsCommentsByIdCardByIdAction
      x-api-path-slug: cardsidcardactionsidactioncomments-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Actions Comments to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idAction
        description: idAction
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Actions
      - Comments
  /cards/{idCard}/attachments:
    get:
      summary: Get Cards Attachments
      description: Get cards attachments.
      operationId: getCardsAttachmentsByIdCard
      x-api-path-slug: cardsidcardattachments-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: query
        name: filter
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Attachments
    post:
      summary: Post Cards Attachments
      description: Post cards attachments.
      operationId: addCardsAttachmentsByIdCard
      x-api-path-slug: cardsidcardattachments-post
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Attachments to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Attachments
  /cards/{idCard}/attachments/{idAttachment}:
    delete:
      summary: Delete Cards Attachments Attachment
      description: Delete cards attachments attachment.
      operationId: deleteCardsAttachmentsByIdCardByIdAttachment
      x-api-path-slug: cardsidcardattachmentsidattachment-delete
      parameters:
      - in: path
        name: idAttachment
        description: idAttachment
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Attachments
      - Attachment
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