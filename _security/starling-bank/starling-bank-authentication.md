---
api_key_in: []
api_specs:
- filename: obie-opendata-swagger.json
  format: json
  label: Starling Open Data API (OBIE Standard)
  slug: starling-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starling-bank/refs/heads/main/openapi/obie-opendata-swagger.json
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Starling Bank Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- personal_access_token
overview: Starling Bank secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and personal_access_token flow(s).
provider_name: Starling Bank
provider_slug: starling-bank
scheme_count: 3
schemes:
- applies_to: Starling bespoke Developer API (api.starlingbank.com/api/v2)
  evidence: RFC 8414 metadata at api.starlingbank.com/.well-known/oauth-authorization-server; unauthenticated GET /api/v2/accounts returns 401 {"error":"invalid_token"} requiring an Authorization bearer header.
  flows:
  - authorizationUrl: https://oauth.starlingbank.com
    flow: authorizationCode
    issuer: https://token-api.starlingbank.com
    response_types_supported:
    - code
    - token
    tokenUrl: https://token-api.starlingbank.com/oauth/access-token
  - flow: personal_access_token
    note: Sandbox and read-only integrations can mint a personal access token in the developer portal instead of running the full authorization-code flow.
  name: BespokeOAuth2
  type: oauth2
- applies_to: All bespoke Developer API calls carry Authorization Bearer access tokens.
  bearerFormat: JWT
  name: BearerToken
  scheme: bearer
  type: http
- applies_to: OBIE Read/Write (AIS/PIS/CBPII) as an FCA-authorised ASPSP
  client_authentication: mutual-TLS (eIDAS/OBIE certificates)
  name: OpenBankingFAPI
  note: Provisioned to enrolled, certificate-holding TPPs; not publicly probeable.
  profile: FAPI 1.0 Advanced
  strong_customer_authentication: PSD2 SCA (redirect / app-to-app)
  type: oauth2
slug: starling-bank-authentication
source_filename: starling-bank-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://api.starlingbank.com/.well-known/oauth-authorization-server + https://developer.starlingbank.com/docs + live 401 probe\ndocs: https://developer.starlingbank.com/docs\nsummary:\n  types: [oauth2, http]\n  http_scheme: bearer\n  oauth2_flows: [authorizationCode, personal_access_token]\n  surfaces:\n  - bespoke Developer API (api.starlingbank.com) — OAuth2 bearer\n  - Open Banking Read/Write (AIS/PIS/CBPII) — FAPI OAuth2/OIDC + mutual-TLS + PSD2 SCA\nschemes:\n- name: BespokeOAuth2\n  type: oauth2\n  applies_to: Starling bespoke Developer API (api.starlingbank.com/api/v2)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth.starlingbank.com\n    tokenUrl: https://token-api.starlingbank.com/oauth/access-token\n    issuer: https://token-api.starlingbank.com\n    response_types_supported: [code, token]\n  - flow: personal_access_token\n    note: Sandbox and read-only integrations can mint a personal\
  \ access token in the\n      developer portal instead of running the full authorization-code flow.\n  evidence: RFC 8414 metadata at api.starlingbank.com/.well-known/oauth-authorization-server;\n    unauthenticated GET /api/v2/accounts returns 401 {\"error\":\"invalid_token\"} requiring\n    an Authorization bearer header.\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: All bespoke Developer API calls carry Authorization Bearer access tokens.\n- name: OpenBankingFAPI\n  type: oauth2\n  applies_to: OBIE Read/Write (AIS/PIS/CBPII) as an FCA-authorised ASPSP\n  profile: FAPI 1.0 Advanced\n  client_authentication: mutual-TLS (eIDAS/OBIE certificates)\n  strong_customer_authentication: PSD2 SCA (redirect / app-to-app)\n  note: Provisioned to enrolled, certificate-holding TPPs; not publicly probeable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starling-bank/refs/heads/main/authentication/starling-bank-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Challenger Bank
- Fintech
- FAPI
---
