---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Get Lists List Cards Filter
  description: Get lists list cards filter.
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
    get:
      summary: Get Cards Attachments Attachment
      description: Get cards attachments attachment.
      operationId: getCardsAttachmentsByIdCardByIdAttachment
      x-api-path-slug: cardsidcardattachmentsidattachment-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
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
  /cards/{idCard}/board:
    get:
      summary: Get Cards Board
      description: Get cards board.
      operationId: getCardsBoardByIdCard
      x-api-path-slug: cardsidcardboard-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
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
      - Board
  /cards/{idCard}/board/{field}:
    get:
      summary: Get Cards Board Field
      description: Get cards board field.
      operationId: getCardsBoardByIdCardByField
      x-api-path-slug: cardsidcardboardfield-get
      parameters:
      - in: path
        name: field
        description: field
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
      - Board
      - Field
  /cards/{idCard}/checkItemStates:
    get:
      summary: Get Cards Checkitemstates
      description: Get cards checkitemstates.
      operationId: getCardsCheckItemStatesByIdCard
      x-api-path-slug: cardsidcardcheckitemstates-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: idCheckItem or state'
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
      - Checkitemstates
  /cards/{idCard}/checklist/{idChecklistCurrent}/checkItem/{idCheckItem}:
    put:
      summary: Put Cards Checklistcurrent Checkitem Checkitem
      description: Put cards checklistcurrent checkitem checkitem.
      operationId: updateCardsChecklistCheckItemByIdCardByIdChecklistCurrentByIdCheckItem
      x-api-path-slug: cardsidcardchecklistidchecklistcurrentcheckitemidcheckitem-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Checklist Id Checklist Current Check Item
          to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idCheckItem
        description: idCheckItem
      - in: path
        name: idChecklistCurrent
        description: idChecklistCurrent
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
      - Checklistcurrent
      - Checkitem
      - Checkitem
  /cards/{idCard}/checklist/{idChecklist}/checkItem:
    post:
      summary: Post Cards Checklist Checkitem
      description: Post cards checklist checkitem.
      operationId: addCardsChecklistCheckItemByIdCardByIdChecklist
      x-api-path-slug: cardsidcardchecklistidchecklistcheckitem-post
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Checklist Check Item to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idChecklist
        description: idChecklist
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
      - Checklist
      - Checkitem
  /cards/{idCard}/checklist/{idChecklist}/checkItem/{idCheckItem}:
    delete:
      summary: Delete Cards Checklist Checkitem Checkitem
      description: Delete cards checklist checkitem checkitem.
      operationId: deleteCardsChecklistCheckItemByIdCardByIdChecklistByIdCheckItem
      x-api-path-slug: cardsidcardchecklistidchecklistcheckitemidcheckitem-delete
      parameters:
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idCheckItem
        description: idCheckItem
      - in: path
        name: idChecklist
        description: idChecklist
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
      - Checklist
      - Checkitem
      - Checkitem
  /cards/{idCard}/checklist/{idChecklist}/checkItem/{idCheckItem}/convertToCard:
    post:
      summary: Post Cards Checklist Checkitem Checkitem Converttocard
      description: Post cards checklist checkitem checkitem converttocard.
      operationId: addCardsChecklistCheckItemConvertToCardByIdCardByIdChecklistByIdCheckItem
      x-api-path-slug: cardsidcardchecklistidchecklistcheckitemidcheckitemconverttocard-post
      parameters:
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idCheckItem
        description: idCheckItem
      - in: path
        name: idChecklist
        description: idChecklist
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
      - Checklist
      - Checkitem
      - Checkitem
      - Converttocard
  /cards/{idCard}/checklist/{idChecklist}/checkItem/{idCheckItem}/name:
    put:
      summary: Put Cards Checklist Checkitem Checkitem Name
      description: Put cards checklist checkitem checkitem name.
      operationId: updateCardsChecklistCheckItemNameByIdCardByIdChecklistByIdCheckItem
      x-api-path-slug: cardsidcardchecklistidchecklistcheckitemidcheckitemname-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Checklist Check Item Name to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idCheckItem
        description: idCheckItem
      - in: path
        name: idChecklist
        description: idChecklist
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
      - Checklist
      - Checkitem
      - Checkitem
      - Name
  /cards/{idCard}/checklist/{idChecklist}/checkItem/{idCheckItem}/pos:
    put:
      summary: Put Cards Checklist Checkitem Checkitem Pos
      description: Put cards checklist checkitem checkitem pos.
      operationId: updateCardsChecklistCheckItemPosByIdCardByIdChecklistByIdCheckItem
      x-api-path-slug: cardsidcardchecklistidchecklistcheckitemidcheckitempos-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Checklist Check Item Pos to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idCheckItem
        description: idCheckItem
      - in: path
        name: idChecklist
        description: idChecklist
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
      - Checklist
      - Checkitem
      - Checkitem
      - Pos
  /cards/{idCard}/checklist/{idChecklist}/checkItem/{idCheckItem}/state:
    put:
      summary: Put Cards Checklist Checkitem Checkitem State
      description: Put cards checklist checkitem checkitem state.
      operationId: updateCardsChecklistCheckItemStateByIdCardByIdChecklistByIdCheckItem
      x-api-path-slug: cardsidcardchecklistidchecklistcheckitemidcheckitemstate-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Checklist Check Item State to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idCheckItem
        description: idCheckItem
      - in: path
        name: idChecklist
        description: idChecklist
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
      - Checklist
      - Checkitem
      - Checkitem
      - State
  /cards/{idCard}/checklists:
    get:
      summary: Get Cards Checklists
      description: Get cards checklists.
      operationId: getCardsChecklistsByIdCard
      x-api-path-slug: cardsidcardchecklists-get
      parameters:
      - in: query
        name: cards
        description: 'One of: all, closed, none, open or visible'
      - in: query
        name: card_fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: checkItems
        description: 'One of: all or none'
      - in: query
        name: checkItem_fields
        description: 'all or a comma-separated list of: name, nameData, pos, state
          or type'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: idBoard, idCard, name or pos'
      - in: query
        name: filter
        description: 'One of: all or none'
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
      - Checklists
    post:
      summary: Post Cards Checklists
      description: Post cards checklists.
      operationId: addCardsChecklistsByIdCard
      x-api-path-slug: cardsidcardchecklists-post
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Checklists to be added
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
      - Checklists
  /cards/{idCard}/checklists/{idChecklist}:
    delete:
      summary: Delete Cards Checklists
      description: Delete cards checklists.
      operationId: deleteCardsChecklistsByIdCardByIdChecklist
      x-api-path-slug: cardsidcardchecklistsidchecklist-delete
      parameters:
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idChecklist
        description: idChecklist
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
      - Checklists
  /cards/{idCard}/closed:
    put:
      summary: Put Cards Closed
      description: Put cards closed.
      operationId: updateCardsClosedByIdCard
      x-api-path-slug: cardsidcardclosed-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Closed to be updated
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
      - Closed
  /cards/{idCard}/desc:
    put:
      summary: Put Cards Desc
      description: Put cards desc.
      operationId: updateCardsDescByIdCard
      x-api-path-slug: cardsidcarddesc-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Desc to be updated
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
      - Desc
  /cards/{idCard}/due:
    put:
      summary: Put Cards Due
      description: Put cards due.
      operationId: updateCardsDueByIdCard
      x-api-path-slug: cardsidcarddue-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Due to be updated
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
      - Due
  /cards/{idCard}/idAttachmentCover:
    put:
      summary: Put Cards Attachmentcover
      description: Put cards attachmentcover.
      operationId: updateCardsIdAttachmentCoverByIdCard
      x-api-path-slug: cardsidcardidattachmentcover-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Id Attachment Cover to be updated
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
      - Attachmentcover
  /cards/{idCard}/idBoard:
    put:
      summary: Put Cards Board
      description: Put cards board.
      operationId: updateCardsIdBoardByIdCard
      x-api-path-slug: cardsidcardidboard-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Id Board to be updated
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
      - Board
  /cards/{idCard}/idLabels:
    post:
      summary: Post Cards Labels
      description: Post cards labels.
      operationId: addCardsIdLabelsByIdCard
      x-api-path-slug: cardsidcardidlabels-post
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Id Labels to be added
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
      - Labels
  /cards/{idCard}/idLabels/{idLabel}:
    delete:
      summary: Delete Cards Labels Label
      description: Delete cards labels label.
      operationId: deleteCardsIdLabelsByIdCardByIdLabel
      x-api-path-slug: cardsidcardidlabelsidlabel-delete
      parameters:
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idLabel
        description: idLabel
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
      - Labels
      - Label
  /cards/{idCard}/idList:
    put:
      summary: Put Cards List
      description: Put cards list.
      operationId: updateCardsIdListByIdCard
      x-api-path-slug: cardsidcardidlist-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Id List to be updated
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
      - List
  /cards/{idCard}/idMembers:
    post:
      summary: Post Cards Members
      description: Post cards members.
      operationId: addCardsIdMembersByIdCard
      x-api-path-slug: cardsidcardidmembers-post
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Id Members to be added
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
      - Members
    put:
      summary: Put Cards Members
      description: Put cards members.
      operationId: updateCardsIdMembersByIdCard
      x-api-path-slug: cardsidcardidmembers-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Id Members to be updated
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
      - Members
  /cards/{idCard}/idMembers/{idMember}:
    delete:
      summary: Delete Cards Members
      description: Delete cards members.
      operationId: deleteCardsIdMembersByIdCardByIdMember
      x-api-path-slug: cardsidcardidmembersidmember-delete
      parameters:
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idMember
        description: idMember
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
      - Members
  /cards/{idCard}/labels:
    post:
      summary: Post Cards Labels
      description: Post cards labels.
      operationId: addCardsLabelsByIdCard
      x-api-path-slug: cardsidcardlabels-post
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Labels to be added
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
      - Labels
    put:
      summary: Put Cards Labels
      description: Put cards labels.
      operationId: updateCardsLabelsByIdCard
      x-api-path-slug: cardsidcardlabels-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Labels to be updated
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
      - Labels
  /cards/{idCard}/labels/{color}:
    delete:
      summary: Delete Cards Labels Color
      description: Delete cards labels color.
      operationId: deleteCardsLabelsByIdCardByColor
      x-api-path-slug: cardsidcardlabelscolor-delete
      parameters:
      - in: path
        name: color
        description: color
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
      - Labels
      - Color
  /cards/{idCard}/list:
    get:
      summary: Get Cards List
      description: Get cards list.
      operationId: getCardsListByIdCard
      x-api-path-slug: cardsidcardlist-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, idBoard, name, pos
          or subscribed'
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
      - List
  /cards/{idCard}/list/{field}:
    get:
      summary: Get Cards List Field
      description: Get cards list field.
      operationId: getCardsListByIdCardByField
      x-api-path-slug: cardsidcardlistfield-get
      parameters:
      - in: path
        name: field
        description: field
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
      - List
      - Field
  /cards/{idCard}/markAssociatedNotificationsRead:
    post:
      summary: Post Cards Markassociatednotificationsread
      description: Post cards markassociatednotificationsread.
      operationId: addCardsMarkAssociatedNotificationsReadByIdCard
      x-api-path-slug: cardsidcardmarkassociatednotificationsread-post
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
      - Markassociatednotificationsread
  /cards/{idCard}/members:
    get:
      summary: Get Cards Members
      description: Get cards members.
      operationId: getCardsMembersByIdCard
      x-api-path-slug: cardsidcardmembers-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
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
      - Members
  /cards/{idCard}/membersVoted:
    get:
      summary: Get Cards Membersvoted
      description: Get cards membersvoted.
      operationId: getCardsMembersVotedByIdCard
      x-api-path-slug: cardsidcardmembersvoted-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
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
      - Membersvoted
    post:
      summary: Post Cards Membersvoted
      description: Post cards membersvoted.
      operationId: addCardsMembersVotedByIdCard
      x-api-path-slug: cardsidcardmembersvoted-post
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Members Voted to be added
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
      - Membersvoted
  /cards/{idCard}/membersVoted/{idMember}:
    delete:
      summary: Delete Cards Membersvoted Member
      description: Delete cards membersvoted member.
      operationId: deleteCardsMembersVotedByIdCardByIdMember
      x-api-path-slug: cardsidcardmembersvotedidmember-delete
      parameters:
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idMember
        description: idMember
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
      - Membersvoted
      - Member
  /cards/{idCard}/name:
    put:
      summary: Put Cards Name
      description: Put cards name.
      operationId: updateCardsNameByIdCard
      x-api-path-slug: cardsidcardname-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Name to be updated
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
      - Name
  /cards/{idCard}/pos:
    put:
      summary: Put Cards Pos
      description: Put cards pos.
      operationId: updateCardsPosByIdCard
      x-api-path-slug: cardsidcardpos-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Pos to be updated
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
      - Pos
  /cards/{idCard}/stickers:
    get:
      summary: Get Cards Stickers
      description: Get cards stickers.
      operationId: getCardsStickersByIdCard
      x-api-path-slug: cardsidcardstickers-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: image, imageScaled, imageUrl,
          left, rotate, top or zIndex'
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
      - Stickers
    post:
      summary: Post Cards Stickers
      description: Post cards stickers.
      operationId: addCardsStickersByIdCard
      x-api-path-slug: cardsidcardstickers-post
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Stickers to be added
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
      - Stickers
  /cards/{idCard}/stickers/{idSticker}:
    delete:
      summary: Delete Cards Stickers Sticker
      description: Delete cards stickers sticker.
      operationId: deleteCardsStickersByIdCardByIdSticker
      x-api-path-slug: cardsidcardstickersidsticker-delete
      parameters:
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idSticker
        description: idSticker
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
      - Stickers
      - Sticker
    get:
      summary: Get Cards Stickers Sticker
      description: Get cards stickers sticker.
      operationId: getCardsStickersByIdCardByIdSticker
      x-api-path-slug: cardsidcardstickersidsticker-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: image, imageScaled, imageUrl,
          left, rotate, top or zIndex'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idSticker
        description: idSticker
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
      - Stickers
      - Sticker
    put:
      summary: Put Cards Stickers Sticker
      description: Put cards stickers sticker.
      operationId: updateCardsStickersByIdCardByIdSticker
      x-api-path-slug: cardsidcardstickersidsticker-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Stickers to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: path
        name: idSticker
        description: idSticker
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
      - Stickers
      - Sticker
  /cards/{idCard}/subscribed:
    put:
      summary: Put Cards Subscribed
      description: Put cards subscribed.
      operationId: updateCardsSubscribedByIdCard
      x-api-path-slug: cardsidcardsubscribed-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Subscribed to be updated
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
      - Subscribed
  /cards/{idCard}/{field}:
    get:
      summary: Get Cards Field
      description: Get cards field.
      operationId: getCardsByIdCardByField
      x-api-path-slug: cardsidcardfield-get
      parameters:
      - in: path
        name: field
        description: field
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
      - Field
  /checklists/{idChecklist}/cards:
    get:
      summary: Get Checklists Cards
      description: Get checklists cards.
      operationId: getChecklistsCardsByIdChecklist
      x-api-path-slug: checklistsidchecklistcards-get
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
        description: 'One of: all, closed, none or open'
      - in: path
        name: idChecklist
        description: idChecklist
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
      - Checklists
      - Cards
  /checklists/{idChecklist}/cards/{filter}:
    get:
      summary: Get Checklists Cards Filter
      description: Get checklists cards filter.
      operationId: getChecklistsCardsByIdChecklistByFilter
      x-api-path-slug: checklistsidchecklistcardsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idChecklist
        description: idChecklist
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
      - Checklists
      - Cards
      - Filter
  /lists/{idList}/cards:
    get:
      summary: Get Lists List Cards
      description: Get lists list cards.
      operationId: getListsCardsByIdList
      x-api-path-slug: listsidlistcards-get
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
        description: 'One of: all, closed, none or open'
      - in: path
        name: idList
        description: idList
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
      - Lists
      - List
      - Cards
    post:
      summary: Post Lists List Cards
      description: Post lists list cards.
      operationId: addListsCardsByIdList
      x-api-path-slug: listsidlistcards-post
      parameters:
      - in: body
        name: body
        description: Attributes of Lists Cards to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idList
        description: idList
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
      - Lists
      - List
      - Cards
  /lists/{idList}/cards/{filter}:
    get:
      summary: Get Lists List Cards Filter
      description: Get lists list cards filter.
      operationId: getListsCardsByIdListByFilter
      x-api-path-slug: listsidlistcardsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idList
        description: idList
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
      - Lists
      - List
      - Cards
      - Filter
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