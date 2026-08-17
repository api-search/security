---
api_key_in:
- header
api_specs:
- filename: termscout-data-openapi.yml
  format: yaml
  label: TermScout Data API
  slug: termscout-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termscout/refs/heads/main/openapi/termscout-data-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Termscout Authentication
name_suffix: Authentication
oauth_flows: []
overview: TermScout secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TermScout
provider_slug: termscout
scheme_count: 2
schemes:
- applied_to: all 11 operations
  description: AWS API Gateway usage-plan key. Sent on every request alongside the Authorization header.
  in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/termscout-data-openapi.yml
  type: apiKey
- applied_to: all 11 operations
  description: 'Bearer-style credential validated by a custom AWS Lambda request authorizer (x-amazon-apigateway-authtype: custom, authorizer type: token, authorizerResultTtlInSeconds: 0 — so every request is re-authorized with no caching).'
  in: header
  name: lambda-api-authorizer
  parameter: Authorization
  sources:
  - openapi/termscout-data-openapi.yml
  type: apiKey
slug: termscout-authentication
source_filename: termscout-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://api.termscout.com/docs\ndocs: https://api.termscout.com/docs\nnote: >-\n  Upgraded from the mechanical derive with the provider's own statement in\n  info.description of the published termscout-data OpenAPI, plus a live\n  anonymous probe of the API host. Both securitySchemes are applied to every\n  one of the 11 operations as an OR list, but the spec text says both are\n  required together: \"All requests require both authentication and an API key.\"\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  requires_both: true\n  self_serve_signup: false\n  onboarding: sales-gated\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: >-\n    AWS API Gateway usage-plan key. Sent on every request alongside the\n    Authorization header.\n  applied_to: all 11 operations\n  sources:\n  - openapi/termscout-data-openapi.yml\n- name: lambda-api-authorizer\n  type: apiKey\n  in:\
  \ header\n  parameter: Authorization\n  description: >-\n    Bearer-style credential validated by a custom AWS Lambda request\n    authorizer (x-amazon-apigateway-authtype: custom, authorizer type: token,\n    authorizerResultTtlInSeconds: 0 — so every request is re-authorized with no\n    caching).\n  applied_to: all 11 operations\n  sources:\n  - openapi/termscout-data-openapi.yml\nprovider_claims:\n- claim: OAuth and Basic auth are supported\n  source: https://api.termscout.com/docs\n  verbatim: 'Oath and Basic auth are supported.'\n  status: unverified\n  note: >-\n    Stated verbatim (with the typo \"Oath\") in info.description, but no oauth2 or\n    http/basic securityScheme is declared anywhere in the spec, and no\n    authorization or token endpoint is published. The declared schemes are both\n    apiKey-in-header. Treated as an undocumented claim, not a conformant OAuth\n    surface — this is why no scopes/ artifact was written.\nx-evidence:\n- fetched: '2026-08-14'\n  url: https://api.termscout.com/openapi.json\n\
  \  http_status: 403\n  body: '{\"message\":\"Missing Authentication Token\"}'\n  note: >-\n    Anonymous request to a non-existent route on the API host. Confirms the API\n    is live and key-gated; AWS API Gateway returns\n    MissingAuthenticationTokenException (x-amzn-errortype header) rather than a\n    401/403 challenge naming a scheme.\n- fetched: '2026-08-14'\n  url: https://api.termscout.com/docs\n  http_status: 200\n  content_type: application/json\n  note: The OpenAPI definition itself is served anonymously; only the data routes are gated.\nkey_acquisition:\n  self_serve: false\n  method: contact sales / demo\n  url: https://www.termscout.com/contact-sales\n  note: >-\n    No developer portal, signup form, or key-issuance page was found on\n    termscout.com, app.termscout.com, or learn.termscout.com. The help centre\n    directs all access questions to a demo booking.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/termscout/refs/heads/main/authentication/termscout-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Legal Tech
- Contract Intelligence
- Contract Certification
- Contract Analysis
- Procurement
- Legal Operations
- Sales Enablement
- AI
- Contract Data
- Document Analysis
---
