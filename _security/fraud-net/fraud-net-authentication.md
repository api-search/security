---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fraud-net-public-apis-openapi.json
  format: json
  label: Fraud.net Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fraud-net/refs/heads/main/openapi/fraud-net-public-apis-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fraud Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fraud.net secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fraud.net
provider_slug: fraud-net
scheme_count: 1
schemes:
- applied: global
  description: 'HTTP Basic Access Authentication. The API key issued by Fraud.net is supplied as the credential pair, base64-encoded and sent as `Authorization: Basic <base64>`. The provider''s own security scheme spells out the four RFC 7617 construction steps.'
  name: basic-auth
  scheme: basic
  sources:
  - openapi/fraud-net-public-apis-openapi.json
  - https://api-docs.fraud.net/docs/public-apis/b2edb775739e6-api-documentation
  type: http
slug: fraud-net-authentication
source_filename: fraud-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: openapi/fraud-net-public-apis-openapi.json\ndocs: https://api-docs.fraud.net/docs/public-apis/b2edb775739e6-api-documentation\nprovider: Fraud.net\nproviderId: fraud-net\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\n  scopes_published: false\n  mtls: false\nschemes:\n  - name: basic-auth\n    type: http\n    scheme: basic\n    applied: global\n    description: >-\n      HTTP Basic Access Authentication. The API key issued by Fraud.net is supplied as the\n      credential pair, base64-encoded and sent as `Authorization: Basic <base64>`. The\n      provider's own security scheme spells out the four RFC 7617 construction steps.\n    sources:\n      - openapi/fraud-net-public-apis-openapi.json\n      - https://api-docs.fraud.net/docs/public-apis/b2edb775739e6-api-documentation\ncredential_issuance:\n  method: portal\n  where: >-\n    \"You can find or generate your API key in the Developer\
  \ section of the Fraud.net\n    Case Management Portal.\" — provider API documentation, Authentication section.\n  self_service: false\n  note: >-\n    There is no public sign-up that yields a key. The portal is reached after a\n    commercial onboarding (https://www.fraud.net/demo-request), so key issuance is\n    sales-gated even though the contract and documentation are fully public.\nobservations:\n  - >-\n    The spec's global `security` requirement references `new-auth`, while the only\n    scheme actually DEFINED in securityDefinitions is `basic-auth`. That is a dangling\n    reference in the provider's published Swagger 2.0 document — recorded as observed,\n    not corrected. The narrative documentation is unambiguous that the mechanism is\n    HTTP Basic.\n  - No OAuth 2.0, OpenID Connect, mutual TLS, or scope surface is published, so\n    scopes/ is deliberately absent for this provider rather than empty.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fraud-net/refs/heads/main/authentication/fraud-net-authentication.yml
summary_line: http · 1 scheme
tags:
- Fraud
- Risk
- Commerce
- Payments
- Security
- Compliance
- Identity
- Banking
- Machine Learning
---
