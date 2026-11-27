---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: google-books-volumes-api-openapi.yml
  format: yaml
  label: Google Books Volumes API
  slug: google-books-volumes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-volumes-api-openapi.yml
- filename: google-books-bookshelves-api-openapi.yml
  format: yaml
  label: Google Books Bookshelves API
  slug: google-books-bookshelves-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-bookshelves-api-openapi.yml
- filename: google-books-cloudloading-api-openapi.yml
  format: yaml
  label: Google Books Cloudloading API
  slug: google-books-cloudloading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-cloudloading-api-openapi.yml
- filename: google-books-dictionary-api-openapi.yml
  format: yaml
  label: Google Books Dictionary API
  slug: google-books-dictionary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-dictionary-api-openapi.yml
- filename: google-books-familysharing-api-openapi.yml
  format: yaml
  label: Google Books Familysharing API
  slug: google-books-familysharing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-familysharing-api-openapi.yml
- filename: google-books-layers-api-openapi.yml
  format: yaml
  label: Google Books Layers API
  slug: google-books-layers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-layers-api-openapi.yml
- filename: google-books-myconfig-api-openapi.yml
  format: yaml
  label: Google Books Myconfig API
  slug: google-books-myconfig-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-myconfig-api-openapi.yml
- filename: google-books-notification-api-openapi.yml
  format: yaml
  label: Google Books Notification API
  slug: google-books-notification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-notification-api-openapi.yml
- filename: google-books-onboarding-api-openapi.yml
  format: yaml
  label: Google Books Onboarding API
  slug: google-books-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-onboarding-api-openapi.yml
- filename: google-books-personalizedstream-api-openapi.yml
  format: yaml
  label: Google Books Personalizedstream API
  slug: google-books-personalizedstream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-personalizedstream-api-openapi.yml
- filename: google-books-promooffer-api-openapi.yml
  format: yaml
  label: Google Books Promooffer API
  slug: google-books-promooffer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-promooffer-api-openapi.yml
- filename: google-books-series-api-openapi.yml
  format: yaml
  label: Google Books Series API
  slug: google-books-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-series-api-openapi.yml
- filename: google-books-mylibrary-api-openapi.yml
  format: yaml
  label: Google Books Books Mylibrary API
  slug: google-books-mylibrary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-books/openapi/google-books-mylibrary-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
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
source_yaml_url: https://artifacts.apis.io/google-books/authentication/google-books-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Books
- Ebooks
- Google
- Library
- Publishing
- Reading
- Search
---
