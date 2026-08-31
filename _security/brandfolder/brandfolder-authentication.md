---
api_key_in: []
api_specs:
- filename: brandfolder-assets-api-openapi.yml
  format: yaml
  label: Brandfolder Assets API
  slug: brandfolder-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-assets-api-openapi.yml
- filename: brandfolder-attachments-api-openapi.yml
  format: yaml
  label: Brandfolder Attachments API
  slug: brandfolder-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-attachments-api-openapi.yml
- filename: brandfolder-binary-upload-api-openapi.yml
  format: yaml
  label: Brandfolder Binary Upload API
  slug: brandfolder-binary-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-binary-upload-api-openapi.yml
- filename: brandfolder-brandfolders-api-openapi.yml
  format: yaml
  label: Brandfolder Brandfolders API
  slug: brandfolder-brandfolders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-brandfolders-api-openapi.yml
- filename: brandfolder-collections-api-openapi.yml
  format: yaml
  label: Brandfolder Collections API
  slug: brandfolder-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-collections-api-openapi.yml
- filename: brandfolder-custom-fields-api-openapi.yml
  format: yaml
  label: Brandfolder Custom Fields API
  slug: brandfolder-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-custom-fields-api-openapi.yml
- filename: brandfolder-invitations-api-openapi.yml
  format: yaml
  label: Brandfolder Invitations API
  slug: brandfolder-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-invitations-api-openapi.yml
- filename: brandfolder-labels-api-openapi.yml
  format: yaml
  label: Brandfolder Labels API
  slug: brandfolder-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-labels-api-openapi.yml
- filename: brandfolder-organizations-api-openapi.yml
  format: yaml
  label: Brandfolder Organizations API
  slug: brandfolder-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-organizations-api-openapi.yml
- filename: brandfolder-sections-api-openapi.yml
  format: yaml
  label: Brandfolder Sections API
  slug: brandfolder-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-sections-api-openapi.yml
- filename: brandfolder-tags-api-openapi.yml
  format: yaml
  label: Brandfolder Tags API
  slug: brandfolder-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-tags-api-openapi.yml
- filename: brandfolder-user-permissions-api-openapi.yml
  format: yaml
  label: Brandfolder User Permissions API
  slug: brandfolder-user-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-user-permissions-api-openapi.yml
- filename: brandfolder-webhooks-api-openapi.yml
  format: yaml
  label: Brandfolder Webhooks API
  slug: brandfolder-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/openapi/brandfolder-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Brandfolder Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brandfolder secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brandfolder
provider_slug: brandfolder
scheme_count: 1
schemes:
- applied: global
  description: API Token.
  name: APIToken
  scheme: bearer
  sources:
  - openapi/brandfolder-openapi-original.yml
  type: http
slug: brandfolder-authentication
source_filename: brandfolder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/brandfolder-openapi-original.yml\ndocs: https://developers.smartsheet.com/api/brandfolder/guides/basics/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  oauth2_flows: []\n  api_key_in: []\nschemes:\n- name: APIToken\n  type: http\n  scheme: bearer\n  description: API Token.\n  applied: global\n  sources:\n  - openapi/brandfolder-openapi-original.yml\nmodel:\n  credential: personal API key (per user)\n  header: 'Authorization: Bearer {BF_API_KEY}'\n  issuance: >\n    Self-service from the signed-in user profile at\n    https://brandfolder.com/profile#integrations - copy the key from the\n    Integrations tab. Requires a Brandfolder account, which requires a sales\n    contract (plans/brandfolder-plans-pricing.yml).\n  authorization: >\n    There are no scopes. The key inherits the issuing user's permissions\n    verbatim: \"Each response to your API calls will only include the resources\n\
  \    that you (or the User whose API key your application is using) can access\n    based on your permissions.\" Least-privilege is achieved by creating a\n    restricted user, not by restricting the token.\n  rotation: null\n  expiry: null\n  multiple_keys: null\n  service_accounts: null\noauth2: false\noauth2_note: >\n  Brandfolder publishes no OAuth 2.0 authorization server for the v4 API.\n  /.well-known/oauth-authorization-server 404s on brandfolder.com. The 200 on\n  developers.smartsheet.com is the docs platform's own OAuth (issuer\n  auth.cloud.redocly.com) governing the portal MCP - it does not issue tokens\n  for the Brandfolder API. No scopes/ artifact is emitted for this provider.\ngaps:\n  - No scopes or permission grants on the credential itself.\n  - No documented key rotation, expiry or revocation procedure.\n  - No machine-to-machine / service-account credential distinct from a human user key.\n  - Keys are long-lived bearer strings; compromise grants the full permission\
  \ set of the issuing user.\nx-evidence:\n  - url: https://developers.smartsheet.com/api/brandfolder/guides/basics/authentication\n    status: 200\n  - url: https://brandfolder.com/.well-known/oauth-authorization-server\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandfolder/refs/heads/main/authentication/brandfolder-authentication.yml
summary_line: http · 1 scheme
tags:
- Digital Asset Management
- DAM
- Brand Management
- Assets
- Media
- Collection
- Smartsheet
---
