# Trello API Testing with Postman

A practice project demonstrating REST API testing with Postman and the Trello API.

## What this collection covers

The collection contains nine requests for working with Trello boards, lists, and cards:

- Get all boards
- Create a board
- Get a single board
- Create a list in a board
- Get all lists in a board
- Create a card
- Update a card name and validate the updated response
- Delete a card
- Delete a board

The requests use collection variables for the base URL, API credentials, and resource IDs. The collection is sanitized for public sharing: the `trelloKey` and `trelloToken` values are intentionally blank.

## Tools and concepts

- Postman collections and variables
- REST API requests using GET, POST, PUT, and DELETE
- Trello API authentication with an API key and token
- Response validation with Postman tests
- Chaining requests by storing and reusing resource IDs

## Setup

1. Download and import `Trello_API_Postman_Collection_Reviewed_Fixed.json` into Postman.
2. Create your own Trello API key and token using Trello's official developer documentation.
3. In the collection variables, set `trelloKey` and `trelloToken` to your own credentials.
4. Run the requests in order where later requests depend on IDs created earlier. The collection scripts save `boardId`, `listId`, and `cardId` as requests create those resources.
5. Review the response and the **Test Results** tab for each request.

## Security note

Never commit a real API key or token to a public repository. Use your own credentials locally in Postman and keep the published collection free of secrets. Requests that create or delete boards and cards change data in your Trello account, so run them only against a test board you are comfortable modifying.

## Project purpose

This is a learning/portfolio project created to practice API testing with Postman. It demonstrates hands-on familiarity with request methods, variables, response checks, and API resource workflows; it is not presented as professional work experience.
