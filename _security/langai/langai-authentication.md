---
api_key_in: []
api_specs:
- filename: langai-documents-api-openapi.yml
  format: yaml
  label: Lang.ai Documents API
  slug: langai-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langai/refs/heads/main/openapi/langai-documents-api-openapi.yml
- filename: langai-projects-api-openapi.yml
  format: yaml
  label: Lang.ai Projects API
  slug: langai-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/langai/refs/heads/main/openapi/langai-projects-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Langai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lang.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lang.ai
provider_slug: langai
scheme_count: 1
schemes:
- description: 'Authenticate your account by including your secret API token in every request as an Authorization: Bearer header. Create a new API token from the Settings section of your Lang.ai instance. Generating a new token invalidates previously issued ones.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/langai-api-openapi.yml
  type: http
slug: langai-authentication
source_filename: langai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://docs.lang.ai/#authentication\ndocs: https://docs.lang.ai/#authentication\nderived_from: openapi/_original/langai-api-openapi.yml\nchecked: '2026-08-14'\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes_published: false\n  scopes_note: >-\n    Lang.ai has no OAuth surface and therefore no scope model. A single static bearer\n    token carries full instance-level authority — there is no way to issue a\n    least-privilege credential, which is the single most consequential authentication\n    fact about this API for an agent deployment.\n  multi_tenant_note: >-\n    Authentication alone is not sufficient to address the API. The base URL is the\n    per-tenant template https://{company}.lang.ai/api/v1, so a caller needs both the\n    bearer token AND the customer's own instance subdomain.\ntoken_lifecycle:\n\
  \  issued_from: Settings section of your Lang.ai instance\n  expiry: not documented\n  rotation: single-active-token\n  rotation_detail: >-\n    \"Keep in mind that generating a new token will invalidate the previously issued\n    ones.\" There is no overlap window, so rotation is a hard cutover: every client must\n    be updated simultaneously or it will start receiving 401.\n  revocation: implicit — issuing a new token revokes all prior tokens\n  provider_warning: >-\n    \"Do not share your secret API tokens in publicly accessible areas such GitHub,\n    client-side code, and so forth.\"\n  applies_to: every request\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authenticate your account by including your secret API token in every request\n    as an Authorization: Bearer header. Create a new API token from the Settings section of\n    your Lang.ai instance. Generating a new token invalidates previously issued ones.'\n  sources:\n  - openapi/langai-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/langai/refs/heads/main/authentication/langai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Natural Language Processing
- Conversation Intelligence
- Customer Support
- Text Classification
- Analytics
- Customer Experience
---
