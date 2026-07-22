---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Simplenexus Authentication
name_suffix: Authentication
oauth_flows: []
overview: SimpleNexus secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SimpleNexus
provider_slug: simplenexus
scheme_count: 1
schemes:
- credentials: API Credentials issued via the developer portal
  credentials_docs: https://developer.ncinomortgage.com/mortgage/docs/obtaining-an-api-key
  documented: true
  name: OAuth2
  sources:
  - https://developer.ncinomortgage.com/mortgage/docs/authentication-1
  token_expiration: true
  type: oauth2
slug: simplenexus-authentication
source_filename: simplenexus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.ncinomortgage.com/mortgage/docs/authentication-1\ndocs: https://developer.ncinomortgage.com/mortgage/docs/authentication-1\nnote: >-\n  SimpleNexus's API is now delivered as the nCino Mortgage API, which explicitly\n  \"replaces the legacy SimpleNexus API.\" The new API uses OAuth 2.0. Exact grant\n  type, token endpoint, header format, and scope list were not exposed in the\n  public docs excerpt (they sit behind the Authentication and \"Obtaining API\n  Credentials\" guides). Captured at the type level from the published docs; not\n  fabricated beyond what the provider states.\nsummary:\n  types: [oauth2]\n  oauth2_flows: []          # documented as an \"Authorization Flow\" but the specific grant was not published in the excerpt\n  api_key_in: []\nschemes:\n  - name: OAuth2\n    type: oauth2\n    documented: true\n    token_expiration: true   # docs state tokens expire (improvement over legacy SimpleNexus\
  \ API)\n    credentials: API Credentials issued via the developer portal\n    credentials_docs: https://developer.ncinomortgage.com/mortgage/docs/obtaining-an-api-key\n    sources: [https://developer.ncinomortgage.com/mortgage/docs/authentication-1]\nlegacy:\n  name: SimpleNexus API (v0-SNAPI)\n  status: deprecated\n  reference: https://developer.ncinomortgage.com/mortgage/v0-SNAPI\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simplenexus/refs/heads/main/authentication/simplenexus-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Mortgage
- Lending
- Fintech
- Financial Services
- Homeownership
- Real Estate
- Webhooks
---
