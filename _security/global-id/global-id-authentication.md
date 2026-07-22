---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Global Id Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Global ID secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Global ID
provider_slug: global-id
scheme_count: 2
schemes:
- description: OAuth2 authorization-code login that lets a relying party authenticate a user with their GlobaliD identity and request identity/verifiable-credential claims.
  evidence: https://github.com/globalid/dev-tooling-examples
  flow: authorizationCode
  name: GlobaliD Connect ("Sign in with GlobaliD")
  sdk: globalid-connect-sdk
  type: oauth2
- description: Server-side toolkits (GidIssuerClient / verifier client) authenticate with a developer-app client ID + client secret to issue and verify credentials.
  evidence: https://github.com/globalid/issuer-toolkit
  flow: clientCredentials
  name: Developer App credentials (issuer/verifier)
  sdks:
  - '@globalid/issuer-toolkit'
  - '@globalid/verifier-toolkit'
  type: oauth2
slug: global-id-authentication
source_filename: global-id-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://developer.global.id/ + https://github.com/globalid/issuer-toolkit +\n  https://github.com/globalid/dev-tooling-examples + npm globalid-connect-sdk /\n  globalid-hydra-helper\ndocs: https://developer.global.id/\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  authorization_server: Ory Hydra (globalid-hydra-helper)\n  credential_source: >-\n    Developer apps created in the GlobaliD developer portal issue a client ID and\n    client secret. There is no self-serve public spec — developer portal access is\n    invitation-based (contact required).\nschemes:\n  - name: GlobaliD Connect (\"Sign in with GlobaliD\")\n    type: oauth2\n    flow: authorizationCode\n    description: >-\n      OAuth2 authorization-code login that lets a relying party authenticate a user\n      with their GlobaliD identity and request identity/verifiable-credential claims.\n    sdk: globalid-connect-sdk\n\
  \    evidence: https://github.com/globalid/dev-tooling-examples\n  - name: Developer App credentials (issuer/verifier)\n    type: oauth2\n    flow: clientCredentials\n    description: >-\n      Server-side toolkits (GidIssuerClient / verifier client) authenticate with a\n      developer-app client ID + client secret to issue and verify credentials.\n    sdks: [\"@globalid/issuer-toolkit\", \"@globalid/verifier-toolkit\"]\n    evidence: https://github.com/globalid/issuer-toolkit\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/global-id/refs/heads/main/authentication/global-id-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Identity
- Digital Identity
- Decentralized Identity
- Self-Sovereign Identity
- Verifiable Credentials
- Authentication
- OAuth
---
