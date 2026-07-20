---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Imply Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Imply secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Imply
provider_slug: imply
scheme_count: 2
schemes:
- description: 'Primary and recommended method. The Polaris API key is passed as the username value in the HTTP Basic Authorization header; no password is provided. API keys never expire, which is why Imply recommends them over OAuth access tokens for programmatic access.

    '
  docs: https://docs.imply.io/polaris/api-keys
  name: ApiKeyBasicAuth
  scheme: basic
  type: http
- description: 'Alternative method. An OAuth access token is passed in the Authorization header. Access tokens are short-lived; Imply discourages them for long-lived integrations in favor of API keys.

    '
  docs: https://docs.imply.io/polaris/oauth
  name: OAuth2Bearer
  type: oauth2
slug: imply-authentication
source_filename: imply-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.imply.io/polaris/auth-overview/\ndocs: https://docs.imply.io/polaris/auth-overview/\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  api_key_scheme: http-basic (API key passed as the Basic-auth username, no password)\n  oauth2_flows: [clientCredentials]\nschemes:\n  - name: ApiKeyBasicAuth\n    type: http\n    scheme: basic\n    description: >\n      Primary and recommended method. The Polaris API key is passed as the\n      username value in the HTTP Basic Authorization header; no password is\n      provided. API keys never expire, which is why Imply recommends them over\n      OAuth access tokens for programmatic access.\n    docs: https://docs.imply.io/polaris/api-keys\n  - name: OAuth2Bearer\n    type: oauth2\n    description: >\n      Alternative method. An OAuth access token is passed in the Authorization\n      header. Access tokens are short-lived; Imply discourages them for\n      long-lived\
  \ integrations in favor of API keys.\n    docs: https://docs.imply.io/polaris/oauth\nnotes: >\n  Derived-from-docs, not from a captured OpenAPI (the Polaris OpenAPI is rendered\n  client-side via Redoc at docs.imply.io/api/polaris/api-reference and was not\n  retrievable as a static file this pass). API keys are managed via the API Keys\n  v1 resource group and carry role-based permissions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imply/refs/heads/main/authentication/imply-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Analytics
- Real-Time Analytics
- Database
- Apache Druid
- Data
- DBaaS
- Streaming
---
