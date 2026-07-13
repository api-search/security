---
api_key_in:
- header
api_specs:
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Documents API
  slug: scrive-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Templates API
  slug: scrive-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Signing API
  slug: scrive-signing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive e-ID Authentication API
  slug: scrive-eid-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Attachments API
  slug: scrive-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Callbacks API
  slug: scrive-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
- filename: scrive-openapi.yml
  format: yaml
  label: Scrive Access Control API
  slug: scrive-access-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/openapi/scrive-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Scrive Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Scrive secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Scrive
provider_slug: scrive
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://oauth2.scrive.com/oauth2/authorization
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://oauth2.scrive.com/oauth2/token
  name: oauth2
  sources:
  - openapi/scrive-openapi.yml
  type: oauth2
- description: OAuth 1.0 or personal access credentials passed in the Authorization header using PLAINTEXT signatures (oauth_consumer_key, oauth_token, oauth_signature).
  in: header
  name: oauth1
  parameter: Authorization
  sources:
  - openapi/scrive-openapi.yml
  type: apiKey
slug: scrive-authentication
source_filename: scrive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scrive-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth2.scrive.com/oauth2/authorization\n    tokenUrl: https://oauth2.scrive.com/oauth2/token\n    scopes: 6\n  sources:\n  - openapi/scrive-openapi.yml\n- name: oauth1\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: OAuth 1.0 or personal access credentials passed in the Authorization header using\n    PLAINTEXT signatures (oauth_consumer_key, oauth_token, oauth_signature).\n  sources:\n  - openapi/scrive-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scrive/refs/heads/main/authentication/scrive-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- E-Signature
- Electronic Signing
- Digital Identity
- e-ID
- BankID
- MitID
- Nordic
- Document Workflow
---
