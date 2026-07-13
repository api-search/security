---
api_key_in:
- query
api_specs:
- filename: books.yml
  format: yaml
  label: Google Books API V1
  slug: google-books
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-books/refs/heads/main/openapi/books.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Books Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Books secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Books
provider_slug: google-books
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/books.yml
  type: oauth2
- in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/books.yml
  type: apiKey
slug: google-books-authentication
source_filename: google-books-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/books.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  sources:\n  - openapi/books.yml\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/books.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-books/refs/heads/main/authentication/google-books-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Books
- eBooks
- Google
- Library
- Publishing
- Reading
- Search
---
