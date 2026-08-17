---
api_key_in:
- header
api_specs:
- filename: convertkit-accounts-api-openapi.yml
  format: yaml
  label: Kit Accounts API
  slug: convertkit-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-accounts-api-openapi.yml
- filename: convertkit-broadcasts-api-openapi.yml
  format: yaml
  label: Kit Broadcasts API
  slug: convertkit-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-broadcasts-api-openapi.yml
- filename: convertkit-custom-fields-api-openapi.yml
  format: yaml
  label: Kit Custom Fields API
  slug: convertkit-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-custom-fields-api-openapi.yml
- filename: convertkit-email-templates-api-openapi.yml
  format: yaml
  label: Kit Email Templates API
  slug: convertkit-email-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-email-templates-api-openapi.yml
- filename: convertkit-forms-api-openapi.yml
  format: yaml
  label: Kit Forms API
  slug: convertkit-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-forms-api-openapi.yml
- filename: convertkit-posts-api-openapi.yml
  format: yaml
  label: Kit Posts API
  slug: convertkit-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-posts-api-openapi.yml
- filename: convertkit-purchases-api-openapi.yml
  format: yaml
  label: Kit Purchases API
  slug: convertkit-purchases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-purchases-api-openapi.yml
- filename: convertkit-segments-api-openapi.yml
  format: yaml
  label: Kit Segments API
  slug: convertkit-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-segments-api-openapi.yml
- filename: convertkit-sequence-emails-api-openapi.yml
  format: yaml
  label: Kit Sequence Emails API
  slug: convertkit-sequence-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-sequence-emails-api-openapi.yml
- filename: convertkit-sequences-api-openapi.yml
  format: yaml
  label: Kit Sequences API
  slug: convertkit-sequences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-sequences-api-openapi.yml
- filename: convertkit-snippets-api-openapi.yml
  format: yaml
  label: Kit Snippets API
  slug: convertkit-snippets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-snippets-api-openapi.yml
- filename: convertkit-subscribers-api-openapi.yml
  format: yaml
  label: Kit Subscribers API
  slug: convertkit-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-subscribers-api-openapi.yml
- filename: convertkit-tags-api-openapi.yml
  format: yaml
  label: Kit Tags API
  slug: convertkit-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-tags-api-openapi.yml
- filename: convertkit-webhooks-api-openapi.yml
  format: yaml
  label: Kit Webhooks API
  slug: convertkit-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/openapi/convertkit-webhooks-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Convertkit Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Kit secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Kit
provider_slug: convertkit
scheme_count: 2
schemes:
- description: Authenticate API requests via an API Key
  in: header
  name: API Key
  parameter: X-Kit-Api-Key
  sources:
  - openapi/convertkit-accounts-api-openapi.yml
  - openapi/convertkit-broadcasts-api-openapi.yml
  - openapi/convertkit-custom-fields-api-openapi.yml
  - openapi/convertkit-email-templates-api-openapi.yml
  - openapi/convertkit-forms-api-openapi.yml
  - openapi/convertkit-posts-api-openapi.yml
  - openapi/convertkit-purchases-api-openapi.yml
  - openapi/convertkit-segments-api-openapi.yml
  - openapi/convertkit-sequence-emails-api-openapi.yml
  - openapi/convertkit-sequences-api-openapi.yml
  - openapi/convertkit-snippets-api-openapi.yml
  - openapi/convertkit-subscribers-api-openapi.yml
  - openapi/convertkit-tags-api-openapi.yml
  - openapi/convertkit-webhooks-api-openapi.yml
  type: apiKey
- description: Authenticate API requests via an OAuth token
  flows:
  - authorizationUrl: https://api.kit.com/v4/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.kit.com/v4/oauth/token
  name: OAuth2
  sources:
  - openapi/convertkit-accounts-api-openapi.yml
  - openapi/convertkit-broadcasts-api-openapi.yml
  - openapi/convertkit-custom-fields-api-openapi.yml
  - openapi/convertkit-email-templates-api-openapi.yml
  - openapi/convertkit-forms-api-openapi.yml
  - openapi/convertkit-posts-api-openapi.yml
  - openapi/convertkit-purchases-api-openapi.yml
  - openapi/convertkit-segments-api-openapi.yml
  - openapi/convertkit-sequence-emails-api-openapi.yml
  - openapi/convertkit-sequences-api-openapi.yml
  - openapi/convertkit-snippets-api-openapi.yml
  - openapi/convertkit-subscribers-api-openapi.yml
  - openapi/convertkit-tags-api-openapi.yml
  - openapi/convertkit-webhooks-api-openapi.yml
  type: oauth2
slug: convertkit-authentication
source_filename: convertkit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/convertkit-accounts-api-openapi.yml, openapi/convertkit-broadcasts-api-openapi.yml, openapi/convertkit-custom-fields-api-openapi.yml,\n  openapi/convertkit-email-templates-api-openapi.yml, openapi/convertkit-forms-api-openapi.yml, openapi/convertkit-posts-api-openapi.yml,\n  openapi/convertkit-purchases-api-openapi.yml, openapi/convertkit-segments-api-openapi.yml, openapi/convertkit-sequence-emails-api-openapi.yml,\n  openapi/convertkit-sequences-api-openapi.yml, openapi/convertkit-snippets-api-openapi.yml, openapi/convertkit-subscribers-api-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: API Key\n  type: apiKey\n  in: header\n  parameter: X-Kit-Api-Key\n  description: Authenticate API requests via an API Key\n  sources:\n  - openapi/convertkit-accounts-api-openapi.yml\n  - openapi/convertkit-broadcasts-api-openapi.yml\n\
  \  - openapi/convertkit-custom-fields-api-openapi.yml\n  - openapi/convertkit-email-templates-api-openapi.yml\n  - openapi/convertkit-forms-api-openapi.yml\n  - openapi/convertkit-posts-api-openapi.yml\n  - openapi/convertkit-purchases-api-openapi.yml\n  - openapi/convertkit-segments-api-openapi.yml\n  - openapi/convertkit-sequence-emails-api-openapi.yml\n  - openapi/convertkit-sequences-api-openapi.yml\n  - openapi/convertkit-snippets-api-openapi.yml\n  - openapi/convertkit-subscribers-api-openapi.yml\n  - openapi/convertkit-tags-api-openapi.yml\n  - openapi/convertkit-webhooks-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.kit.com/v4/oauth/authorize\n    tokenUrl: https://api.kit.com/v4/oauth/token\n    scopes: 2\n  description: Authenticate API requests via an OAuth token\n  sources:\n  - openapi/convertkit-accounts-api-openapi.yml\n  - openapi/convertkit-broadcasts-api-openapi.yml\n  - openapi/convertkit-custom-fields-api-openapi.yml\n\
  \  - openapi/convertkit-email-templates-api-openapi.yml\n  - openapi/convertkit-forms-api-openapi.yml\n  - openapi/convertkit-posts-api-openapi.yml\n  - openapi/convertkit-purchases-api-openapi.yml\n  - openapi/convertkit-segments-api-openapi.yml\n  - openapi/convertkit-sequence-emails-api-openapi.yml\n  - openapi/convertkit-sequences-api-openapi.yml\n  - openapi/convertkit-snippets-api-openapi.yml\n  - openapi/convertkit-subscribers-api-openapi.yml\n  - openapi/convertkit-tags-api-openapi.yml\n  - openapi/convertkit-webhooks-api-openapi.yml\ndocs: https://developers.kit.com/api-reference/authentication\nsearched_note: Upgraded from the mechanical derive with Kit's published auth docs and the live RFC 8414\n  / RFC 9728 well-known documents. Note the OpenAPI oauth2 endpoint URLs (api.kit.com/v4/oauth/*) disagree\n  with the live authorization-server metadata (authorize on app.kit.com, no /v4 prefix) — see scopes/convertkit-scopes.yml.\nlive_metadata:\n  authorization_server: https://api.kit.com/.well-known/oauth-authorization-server\n\
  \  protected_resource: https://api.kit.com/.well-known/oauth-protected-resource\n  probed: '2026-08-13'\n  http_status: 200\n  issuer: https://api.kit.com\n  authorization_endpoint: https://app.kit.com/oauth/authorize\n  token_endpoint: https://api.kit.com/oauth/token\n  revocation_endpoint: https://api.kit.com/oauth/revoke\n  registration_endpoint: https://app.kit.com/oauth/register\n  dynamic_client_registration: true\n  pkce: S256\n  grant_types_supported:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods_supported:\n  - client_secret_post\n  - none\nusage_policy:\n  api_key:\n    header: X-Kit-Api-Key\n    intended_use: Personal automation and pre-launch testing only\n    rate_limit: 120 requests / rolling 60s\n    restrictions: Rejected by every /v4/bulk/ endpoint and by POST /v4/purchases\n    retrievability: Shown once at creation in account settings > Developer; not retrievable later\n  oauth:\n    required_for: Any app published to the Kit App Store, all\
  \ bulk endpoints, purchase creation, and the\n      Kit MCP\n    rate_limit: 600 requests / rolling 60s\n    flows:\n    - authorization_code\n    - authorization_code + PKCE (SPAs and mobile)\n    - refresh_token\n    refresh_token_rotation: Single-use since 2026-05-20; each refresh issues a new refresh token and revokes\n      the previous. Reuse returns invalid_grant.\n    docs:\n    - https://developers.kit.com/api-reference/oauth-refresh-token-flow\n    - https://developers.kit.com/api-reference/oauth-proof-key-for-code-exchange-flow\n    - https://developers.kit.com/api-reference/oauth-token-revocation\nscopes_artifact: scopes/convertkit-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convertkit/refs/heads/main/authentication/convertkit-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Email Marketing
- Creator Economy
- Subscribers
- Automation
- Newsletters
- Sequences
- Forms
- Broadcasts
- Webhooks
- MCP
- Agents
- OAuth
- Marketing Automation
- Landing Pages
- Segmentation
- Email Campaigns
- SaaS
- Commerce
---
