---
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cerby Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cerby secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cerby
provider_slug: cerby
scheme_count: 3
schemes:
- applies_to: Cerby API (https://{my-workspace}.cerby.com/api/v1/)
  authorization_model: Cerby layers role-based access control on top of the key. A key resolves to the user who created it, so it can only reach items that user holds the required workspace and item role on. All-Access Mode, which lets workspace Owners and Super Admins see every item in the web app, is explicitly NOT honored by the API — API requests return only items the key's user has the Owner role on, regardless of the All-Access Mode setting.
  description: Every request to the Cerby API must carry the X-API-Key header. Keys are generated and retrieved only from the Cerby web app after authenticating through the corporate identity provider (Okta, Entra ID, OneLogin) that fronts the workspace. Keys are scoped — see scopes/cerby-scopes.yml — and the scopes selected at generation time determine which endpoints and data the key can reach.
  docs: https://help.cerby.com/developer-tools/cerby-api/generate-an-api-key
  failure_modes:
  - condition: expired key, or key lacking the scopes for the endpoint
    status: 401
  - condition: key valid but without permission for the requested operation
    status: 403
  in: header
  name: CerbyApiKey
  parameter_name: X-API-Key
  source: https://developer.cerby.com/#authentication
  type: apiKey
- applies_to: Cerby CLI
  description: The Cerby CLI authenticates with a bearer token retrieved from the Cerby web app rather than with an X-API-Key. The CLI additionally requires the machine to be registered as a trusted device before it can sync and decrypt vault material locally.
  docs: https://help.cerby.com/developer-tools/cerby-api/retrieve-a-bearer-token
  name: CerbyBearerToken
  scheme: bearer
  source: https://help.cerby.com/developer-tools/cerby-api/explore-api-keys-and-bearer-tokens
  type: http
- applies_to: Cerby SCIM 2.0 (https://api.cerby.com/v1/scim/v2)
  description: SCIM provisioning from an identity provider uses a separate SCIM API authentication token, generated and regenerable from the Cerby web app. It is distinct from the Cerby API key and does not carry API-key scopes.
  docs: https://help.cerby.com/setup-and-admin/workspace-identity-federation/retrieve-the-scim-api-authentication-token-from-cerby
  in: header
  name: CerbyScimToken
  parameter_name: Authorization
  source: https://help.cerby.com/llms.txt
  type: apiKey
slug: cerby-authentication
source_filename: cerby-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://developer.cerby.com/#authentication\ndocs: https://help.cerby.com/developer-tools/cerby-api/explore-api-keys-and-bearer-tokens\nnote: >-\n  Cerby publishes no OpenAPI document, so this profile is read from the published\n  developer portal and help-center articles rather than derived from\n  securitySchemes. Nothing here is inferred.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- name: CerbyApiKey\n  type: apiKey\n  in: header\n  parameter_name: X-API-Key\n  applies_to: Cerby API (https://{my-workspace}.cerby.com/api/v1/)\n  description: >-\n    Every request to the Cerby API must carry the X-API-Key header. Keys are\n    generated and retrieved only from the Cerby web app after authenticating\n    through the corporate identity provider (Okta, Entra ID, OneLogin) that\n    fronts the workspace. Keys\
  \ are scoped — see scopes/cerby-scopes.yml — and\n    the scopes selected at generation time determine which endpoints and data\n    the key can reach.\n  authorization_model: >-\n    Cerby layers role-based access control on top of the key. A key resolves to\n    the user who created it, so it can only reach items that user holds the\n    required workspace and item role on. All-Access Mode, which lets workspace\n    Owners and Super Admins see every item in the web app, is explicitly NOT\n    honored by the API — API requests return only items the key's user has the\n    Owner role on, regardless of the All-Access Mode setting.\n  failure_modes:\n  - condition: expired key, or key lacking the scopes for the endpoint\n    status: 401\n  - condition: key valid but without permission for the requested operation\n    status: 403\n  docs: https://help.cerby.com/developer-tools/cerby-api/generate-an-api-key\n  source: https://developer.cerby.com/#authentication\n- name: CerbyBearerToken\n\
  \  type: http\n  scheme: bearer\n  applies_to: Cerby CLI\n  description: >-\n    The Cerby CLI authenticates with a bearer token retrieved from the Cerby web\n    app rather than with an X-API-Key. The CLI additionally requires the machine\n    to be registered as a trusted device before it can sync and decrypt vault\n    material locally.\n  docs: https://help.cerby.com/developer-tools/cerby-api/retrieve-a-bearer-token\n  source: https://help.cerby.com/developer-tools/cerby-api/explore-api-keys-and-bearer-tokens\n- name: CerbyScimToken\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  applies_to: Cerby SCIM 2.0 (https://api.cerby.com/v1/scim/v2)\n  description: >-\n    SCIM provisioning from an identity provider uses a separate SCIM API\n    authentication token, generated and regenerable from the Cerby web app. It\n    is distinct from the Cerby API key and does not carry API-key scopes.\n  docs: https://help.cerby.com/setup-and-admin/workspace-identity-federation/retrieve-the-scim-api-authentication-token-from-cerby\n\
  \  source: https://help.cerby.com/llms.txt\nkey_management:\n  generated_in: Cerby web app (My Profile > Dev Tools)\n  scopes_selectable_at_creation: true\n  scopes_updatable: true\n  viewable: true\n  revocable: true\n  expiring: true\n  docs:\n  - https://help.cerby.com/developer-tools/cerby-api/generate-an-api-key\n  - https://help.cerby.com/developer-tools/cerby-api/update-the-scopes-of-an-api-key\n  - https://help.cerby.com/developer-tools/cerby-api/view-the-details-of-an-api-key\n  - https://help.cerby.com/developer-tools/cerby-api/delete-an-api-key\nguidance_published:\n- Do not share API keys in public repositories or client-side code.\n- Keys grant access to workspace data and are treated as sensitive resources.\nwebhook_authentication:\n  direction: inbound-to-customer\n  mechanism: request signing, not an API key\n  see: asyncapi/cerby-webhooks.yml\nx-evidence:\n- url: https://developer.cerby.com/\n  http_status: 200\n  fetched: '2026-08-09'\n- url: https://help.cerby.com/developer-tools/cerby-api/explore-api-keys-and-bearer-tokens.md\n\
  \  http_status: 200\n  fetched: '2026-08-09'\n- url: https://help.cerby.com/developer-tools/cerby-api/generate-an-api-key.md\n  http_status: 200\n  fetched: '2026-08-09'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerby/refs/heads/main/authentication/cerby-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Identity
- Access Management
- Security
- Password Management
- Provisioning
- SCIM
- Identity Governance
- Nonfederated Applications
- Automation
- Webhooks
---
