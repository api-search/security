---
api_key_in: []
api_specs:
- filename: swan-io.postman_collection.json
  format: json
  label: Swan Accounts API
  slug: swan-io-accounts-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/swan-io/refs/heads/main/collections/swan-io.postman_collection.json
- filename: swan-io.postman_collection.json
  format: json
  label: Swan Account Memberships API
  slug: swan-io-account-memberships-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/swan-io/refs/heads/main/collections/swan-io.postman_collection.json
- filename: swan-io.postman_collection.json
  format: json
  label: Swan Cards API
  slug: swan-io-cards-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/swan-io/refs/heads/main/collections/swan-io.postman_collection.json
- filename: swan-io.postman_collection.json
  format: json
  label: Swan Payments API
  slug: swan-io-payments-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/swan-io/refs/heads/main/collections/swan-io.postman_collection.json
- filename: swan-io.postman_collection.json
  format: json
  label: Swan Transactions API
  slug: swan-io-transactions-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/swan-io/refs/heads/main/collections/swan-io.postman_collection.json
- filename: swan-io.postman_collection.json
  format: json
  label: Swan Onboarding API
  slug: swan-io-onboarding-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/swan-io/refs/heads/main/collections/swan-io.postman_collection.json
- filename: swan-io.postman_collection.json
  format: json
  label: Swan Users and Consents API
  slug: swan-io-users-consents-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/swan-io/refs/heads/main/collections/swan-io.postman_collection.json
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: documented
name: Swan Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swan secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Swan
provider_slug: swan-io
scheme_count: 3
schemes:
- description: 'Server-to-server access. Exchange your Project Client ID and Client Secret (from the Swan dashboard under Developers > API) for an access token, then send it as `Authorization: Bearer $ACCESS_TOKEN`. Used for Partner API calls that act on behalf of the Project.'
  flow: clientCredentials
  name: oauth2ClientCredentials
  sources:
  - https://docs.swan.io/api/authentication
  - https://swan-io.github.io/swan-partner-frontend/oauth2/
  tokenUrl: https://oauth.swan.io/oauth2/token
  type: oauth2
- authorizationUrl: https://oauth.swan.io/oauth2/auth
  description: 'User access tokens. Redirect the user through Swan''s OAuth2 authorization-code flow to obtain a token that acts on behalf of that user (for example to read their account or approve consents). Sent as `Authorization: Bearer $ACCESS_TOKEN`.'
  flow: authorizationCode
  name: oauth2AuthorizationCode
  sources:
  - https://docs.swan.io/api/authentication
  - https://swan-io.github.io/swan-partner-frontend/oauth2/
  tokenUrl: https://oauth.swan.io/oauth2/token
  type: oauth2
- description: 'All GraphQL requests carry the OAuth2 access token in an `Authorization: Bearer` header. Calls are backend-only - Swan blocks API requests originating directly from a frontend. Tokens, credentials, and URLs do not work across the Sandbox and Live environments.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.swan.io/api/authentication
  type: http
slug: swan-io-authentication
source_filename: swan-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: https://docs.swan.io/api/authentication\nsummary:\n  types:\n  - oauth2\n  - http\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://oauth.swan.io/oauth2/token\n  description: 'Server-to-server access. Exchange your Project Client ID and Client\n    Secret (from the Swan dashboard under Developers > API) for an access token,\n    then send it as `Authorization: Bearer $ACCESS_TOKEN`. Used for Partner API\n    calls that act on behalf of the Project.'\n  sources:\n  - https://docs.swan.io/api/authentication\n  - https://swan-io.github.io/swan-partner-frontend/oauth2/\n- name: oauth2AuthorizationCode\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://oauth.swan.io/oauth2/auth\n  tokenUrl: https://oauth.swan.io/oauth2/token\n  description: 'User access tokens. Redirect the user through Swan''s OAuth2\n    authorization-code flow to obtain a token that\
  \ acts on behalf of that user\n    (for example to read their account or approve consents). Sent as\n    `Authorization: Bearer $ACCESS_TOKEN`.'\n  sources:\n  - https://docs.swan.io/api/authentication\n  - https://swan-io.github.io/swan-partner-frontend/oauth2/\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'All GraphQL requests carry the OAuth2 access token in an\n    `Authorization: Bearer` header. Calls are backend-only - Swan blocks API\n    requests originating directly from a frontend. Tokens, credentials, and URLs\n    do not work across the Sandbox and Live environments.'\n  sources:\n  - https://docs.swan.io/api/authentication\nnotes: >-\n  Swan authorization is scoped to a partner Project and, for many mutations,\n  additionally gated by a Strong Customer Authentication \"consent\": sensitive\n  operations (add memberships, issue cards, initiate payments) return a consent\n  object with a Swan-hosted consentUrl the user must approve before the operation\n\
  \  executes. The exact OAuth2 auth/token paths under https://oauth.swan.io/oauth2\n  should be confirmed against the live dashboard; the token exchange base is\n  documented as POST https://oauth.swan.io/oauth2.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swan-io/refs/heads/main/authentication/swan-io-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Embedded Banking
- Banking as a Service
- BaaS
- Payments
- Accounts
- Cards
- IBAN
- SEPA
- Europe
- France
- Fintech
- GraphQL
---
