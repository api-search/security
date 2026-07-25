---
api_key_in: []
api_specs:
- filename: wefunder-activity-api-openapi.yml
  format: yaml
  label: Wefunder Activity API
  slug: wefunder-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-activity-api-openapi.yml
- filename: wefunder-attribution-api-openapi.yml
  format: yaml
  label: Wefunder Attribution API
  slug: wefunder-attribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-attribution-api-openapi.yml
- filename: wefunder-attribution-partners-api-openapi.yml
  format: yaml
  label: Wefunder Attribution Partners API
  slug: wefunder-attribution-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-attribution-partners-api-openapi.yml
- filename: wefunder-attribution-webhooks-api-openapi.yml
  format: yaml
  label: Wefunder Attribution Webhooks API
  slug: wefunder-attribution-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-attribution-webhooks-api-openapi.yml
- filename: wefunder-campaigns-api-openapi.yml
  format: yaml
  label: Wefunder Campaigns API
  slug: wefunder-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-campaigns-api-openapi.yml
- filename: wefunder-explore-api-openapi.yml
  format: yaml
  label: Wefunder Explore API
  slug: wefunder-explore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-explore-api-openapi.yml
- filename: wefunder-intents-api-openapi.yml
  format: yaml
  label: Wefunder Intents API
  slug: wefunder-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-intents-api-openapi.yml
- filename: wefunder-investments-api-openapi.yml
  format: yaml
  label: Wefunder Investments API
  slug: wefunder-investments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-investments-api-openapi.yml
- filename: wefunder-syndicate-deals-api-openapi.yml
  format: yaml
  label: Wefunder Syndicate Deals API
  slug: wefunder-syndicate-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-syndicate-deals-api-openapi.yml
- filename: wefunder-syndicate-members-api-openapi.yml
  format: yaml
  label: Wefunder Syndicate Members API
  slug: wefunder-syndicate-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-syndicate-members-api-openapi.yml
- filename: wefunder-syndicate-statistics-api-openapi.yml
  format: yaml
  label: Wefunder Syndicate Statistics API
  slug: wefunder-syndicate-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-syndicate-statistics-api-openapi.yml
- filename: wefunder-syndicates-api-openapi.yml
  format: yaml
  label: Wefunder Syndicates API
  slug: wefunder-syndicates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-syndicates-api-openapi.yml
- filename: wefunder-users-api-openapi.yml
  format: yaml
  label: Wefunder Users API
  slug: wefunder-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/openapi/wefunder-users-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Wefunder Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Wefunder secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Wefunder
provider_slug: wefunder
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization with access tokens
  flows:
  - authorizationUrl: https://wefunder.com/oauth/authorize
    flow: authorizationCode
    scopes: 14
    tokenUrl: https://wefunder.com/oauth/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://wefunder.com/oauth/token
  name: bearerAuth
  sources:
  - openapi/wefunder-openapi-original.yml
  type: oauth2
slug: wefunder-authentication
source_filename: wefunder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/wefunder-openapi-original.yml + https://wefunder.com/.well-known/oauth-authorization-server + https://github.com/Wefunder/wefunder-node\ndocs: https://docs.wefunder.com/api-reference\nnotes: >-\n  OAuth 2.0 bearer tokens. Live RFC 8414 metadata at\n  /.well-known/oauth-authorization-server (issuer https://wefunder.com) advertises\n  authorization_code + refresh_token grants, PKCE S256, token_endpoint_auth_methods\n  [none, client_secret_post], and dynamic client registration at\n  https://wefunder.com/oauth/register. The SDK's token host is\n  https://api.wefunder.com/oauth (routes sandbox vs live by pk_test_/pk_live_\n  credential mode); sandbox consent at https://oauth.wefunder-sandbox.com/oauth.\n  Refresh tokens rotate on every refresh. client_credentials tokens hold read:public\n  only; user-context scopes require authorization_code + PKCE.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n\
  \  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wefunder.com/oauth/authorize\n    tokenUrl: https://wefunder.com/oauth/token\n    scopes: 14\n  - flow: clientCredentials\n    tokenUrl: https://wefunder.com/oauth/token\n    scopes: 1\n  description: OAuth 2.0 authorization with access tokens\n  sources:\n  - openapi/wefunder-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wefunder/refs/heads/main/authentication/wefunder-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Crowdfunding
- Equity Crowdfunding
- Investing
- Fintech
- Startups
- Fundraising
- Syndicates
- Regulation Crowdfunding
---
