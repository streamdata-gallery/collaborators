---
swagger: "2.0"
x-collection-name: GitHub
x-complete: 0
info:
  title: Github Put Repos Owner Repo Collaborators User
  description: Add collaborator.
  termsOfService: https://help.github.com/articles/github-terms-of-service/#b-api-terms
  version: 1.0.0
host: api.github.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /repos/{owner}/{repo}/collaborators:
    get:
      summary: Get Repos Owner Repo Collaborators
      description: |-
        List.
        When authenticating as an organization owner of an organization-owned
        repository, all organization owners are included in the list of
        collaborators. Otherwise, only users with access to the repository are
        returned in the collaborators list.
      operationId: listwhen-authenticating-as-an-organization-owner-of-an-organizationownedrepository-all-organization-
      x-api-path-slug: reposownerrepocollaborators-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Collaborators
  /repos/{owner}/{repo}/collaborators/{user}:
    delete:
      summary: Delete Repos Owner Repo Collaborators User
      description: Remove collaborator.
      operationId: remove-collaborator
      x-api-path-slug: reposownerrepocollaboratorsuser-delete
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      - in: path
        name: user
        description: Login of the user
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Collaborators
      - User
    get:
      summary: Get Repos Owner Repo Collaborators User
      description: Check if user is a collaborator
      operationId: check-if-user-is-a-collaborator
      x-api-path-slug: reposownerrepocollaboratorsuser-get
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      - in: path
        name: user
        description: Login of the user
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Collaborators
      - User
    put:
      summary: Put Repos Owner Repo Collaborators User
      description: Add collaborator.
      operationId: add-collaborator
      x-api-path-slug: reposownerrepocollaboratorsuser-put
      parameters:
      - in: header
        name: Accept
        description: Is used to set specified media type
      - in: query
        name: access_token
        description: Your Github OAuth token
      - in: path
        name: owner
        description: Name of repository owner
      - in: path
        name: repo
        description: Name of repository
      - in: path
        name: user
        description: Login of the user
      responses:
        200:
          description: OK
      tags:
      - Repos
      - Owner
      - Repo
      - Collaborators
      - User
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