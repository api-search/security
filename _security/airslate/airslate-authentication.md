---
api_key_in: []
api_specs:
- filename: airslate-document-fields-api-openapi.yml
  format: yaml
  label: airSlate Document Fields API
  slug: airslate-document-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-document-fields-api-openapi.yml
- filename: airslate-document-groups-api-openapi.yml
  format: yaml
  label: airSlate Document Groups API
  slug: airslate-document-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-document-groups-api-openapi.yml
- filename: airslate-documents-api-openapi.yml
  format: yaml
  label: airSlate Documents API
  slug: airslate-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-documents-api-openapi.yml
- filename: airslate-embedded-api-openapi.yml
  format: yaml
  label: airSlate Embedded API
  slug: airslate-embedded-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-embedded-api-openapi.yml
- filename: airslate-folders-api-openapi.yml
  format: yaml
  label: airSlate Folders API
  slug: airslate-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-folders-api-openapi.yml
- filename: airslate-invites-api-openapi.yml
  format: yaml
  label: airSlate Invites API
  slug: airslate-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-invites-api-openapi.yml
- filename: airslate-oauth-api-openapi.yml
  format: yaml
  label: airSlate OAuth API
  slug: airslate-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-oauth-api-openapi.yml
- filename: airslate-smart-fields-api-openapi.yml
  format: yaml
  label: airSlate Smart Fields API
  slug: airslate-smart-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-smart-fields-api-openapi.yml
- filename: airslate-templates-api-openapi.yml
  format: yaml
  label: airSlate Templates API
  slug: airslate-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-templates-api-openapi.yml
- filename: airslate-users-api-openapi.yml
  format: yaml
  label: airSlate Users API
  slug: airslate-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-users-api-openapi.yml
- filename: airslate-webhooks-api-openapi.yml
  format: yaml
  label: airSlate Webhooks API
  slug: airslate-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/openapi/airslate-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Airslate Authentication
name_suffix: Authentication
oauth_flows: []
overview: airSlate secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: airSlate
provider_slug: airslate
scheme_count: 2
schemes:
- description: 'HTTP Basic auth carrying the application Basic Token (base64 of

    client_id:client_secret) used against POST /oauth2/token.'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/airslate-openapi.yml
  type: http
- description: 'OAuth 2.0 bearer access token issued by /oauth2/token. Required on

    all resource endpoints.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/airslate-openapi.yml
  type: http
slug: airslate-authentication
source_filename: airslate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/airslate-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic auth carrying the application Basic Token (base64 of\n    client_id:client_secret) used against POST /oauth2/token.\n  sources:\n  - openapi/airslate-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    OAuth 2.0 bearer access token issued by /oauth2/token. Required on\n    all resource endpoints.\n  sources:\n  - openapi/airslate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/authentication/airslate-authentication.yml
summary_line: http · 2 schemes
tags:
- Document Automation
- E-Signature
- Workflows
- PDF
- No-Code
- Artificial Intelligence
---
