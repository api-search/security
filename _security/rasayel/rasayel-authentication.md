---
api_key_in:
- header
api_specs:
- filename: rasayel-rest-openapi.yml
  format: yaml
  label: Rasayel REST API
  slug: rasayel-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasayel/refs/heads/main/openapi/rasayel-rest-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Rasayel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rasayel secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rasayel
provider_slug: rasayel
scheme_count: 1
schemes:
- description: 'Rasayel authenticates REST requests with an API key. Create a key on the API management page (Settings > API management) and copy its "Basic Auth Value". Send that value in the Authorization header as `Authorization: Basic {token}` on every request.'
  format: Basic {token}
  in: header
  name: basicToken
  parameter: Authorization
  sources:
  - openapi/rasayel-rest-openapi.yml
  type: apiKey
slug: rasayel-authentication
source_filename: rasayel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://rest.developers.rasayel.io/ (public Postman collection docs)\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: basicToken\n    type: apiKey\n    in: header\n    parameter: Authorization\n    format: \"Basic {token}\"\n    description: >-\n      Rasayel authenticates REST requests with an API key. Create a key on the\n      API management page (Settings > API management) and copy its \"Basic Auth\n      Value\". Send that value in the Authorization header as `Authorization:\n      Basic {token}` on every request.\n    sources: [openapi/rasayel-rest-openapi.yml]\nscopes:\n  - scope: read\n    description: Read-only operations (fetch templates, contacts, conversations, etc).\n  - scope: read-write\n    description: Any read or write operation (send a message, create a contact, etc).\nimpersonation:\n  header: X_On_Behalf_Of\n  description: >-\n    Optional header to act on behalf\
  \ of a specific user; set it to that user's\n    ID. The ID is found on the user's profile settings page.\ndocs: https://rest.developers.rasayel.io/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rasayel/refs/heads/main/authentication/rasayel-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- WhatsApp
- Messaging
- Business Messaging
- Sales
- CRM
- Customer Communication
- Conversational Commerce
- API
---
