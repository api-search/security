---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'The public FTC API (https://api.ftc.gov/v0) is fronted by api.data.gov (the GSA-run API Umbrella gateway). Every request must carry an api.data.gov API key. There is no OAuth, no OpenID Connect, no mTLS and no per-user token: one shared key per consumer, self-issued through the api.data.gov signup form the FTC developer page links to. Verified live on 2026-09-09 — an unkeyed request to https://api.ftc.gov/openapi.json returned HTTP 403 with {"error":{"code":"API_KEY_MISSING"}}.'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Federal Trade Commission Authentication
name_suffix: Authentication
oauth_flows: []
overview: Federal Trade Commission declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Federal Trade Commission
provider_slug: federal-trade-commission
scheme_count: 3
schemes:
- applies_to:
  - https://api.ftc.gov/v0/dnc-complaints
  - https://api.ftc.gov/v0/hsr-early-termination-notices
  description: api.data.gov key passed as the api_key query-string parameter. This is the form the FTC's own documented examples use (…/v0/dnc-complaints?api_key=DEMO_KEY).
  id: api-data-gov-key-query
  in: query
  name: api_key
  source: https://www.ftc.gov/developer
  type: apiKey
- applies_to:
  - https://api.ftc.gov/v0/dnc-complaints
  - https://api.ftc.gov/v0/hsr-early-termination-notices
  description: The same api.data.gov key passed in the X-Api-Key request header. Preferred over the query parameter because the key does not then appear in logs or referrers.
  id: api-data-gov-key-header
  in: header
  name: X-Api-Key
  source: https://www.ftc.gov/developer/api/v0/endpoints/hsr-early-termination-notices
  type: apiKey
- description: api.data.gov also accepts the key as the HTTP Basic username with an empty password. Documented by the gateway operator, not by the FTC.
  id: api-data-gov-key-basic
  scheme: basic
  source: https://api.data.gov/docs/developer-manual/
  type: http
slug: federal-trade-commission-authentication
source_filename: federal-trade-commission-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: https://www.ftc.gov/developer\nspecification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Federal Trade Commission\nproviderId: federal-trade-commission\ndocs:\n  - https://www.ftc.gov/developer\n  - https://www.ftc.gov/developer/api/v0/endpoints/do-not-call-dnc-reported-calls-data-api\n  - https://api.data.gov/docs/developer-manual/\ndescription: >-\n  The public FTC API (https://api.ftc.gov/v0) is fronted by api.data.gov (the GSA-run\n  API Umbrella gateway). Every request must carry an api.data.gov API key. There is no\n  OAuth, no OpenID Connect, no mTLS and no per-user token: one shared key per consumer,\n  self-issued through the api.data.gov signup form the FTC developer page links to.\n  Verified live on 2026-09-09 — an unkeyed request to https://api.ftc.gov/openapi.json\n  returned HTTP 403 with {\"error\":{\"code\":\"API_KEY_MISSING\"}}.\nschemes:\n  - id: api-data-gov-key-query\n    type: apiKey\n\
  \    in: query\n    name: api_key\n    description: >-\n      api.data.gov key passed as the api_key query-string parameter. This is the form the\n      FTC's own documented examples use (…/v0/dnc-complaints?api_key=DEMO_KEY).\n    applies_to:\n      - https://api.ftc.gov/v0/dnc-complaints\n      - https://api.ftc.gov/v0/hsr-early-termination-notices\n    source: https://www.ftc.gov/developer\n  - id: api-data-gov-key-header\n    type: apiKey\n    in: header\n    name: X-Api-Key\n    description: >-\n      The same api.data.gov key passed in the X-Api-Key request header. Preferred over the\n      query parameter because the key does not then appear in logs or referrers.\n    applies_to:\n      - https://api.ftc.gov/v0/dnc-complaints\n      - https://api.ftc.gov/v0/hsr-early-termination-notices\n    source: https://www.ftc.gov/developer/api/v0/endpoints/hsr-early-termination-notices\n  - id: api-data-gov-key-basic\n    type: http\n    scheme: basic\n    description: >-\n      api.data.gov\
  \ also accepts the key as the HTTP Basic username with an empty password.\n      Documented by the gateway operator, not by the FTC.\n    source: https://api.data.gov/docs/developer-manual/\nkey_issuance:\n  issuer: api.data.gov (U.S. General Services Administration)\n  signup: https://api.data.gov/signup/\n  self_service: true\n  cost: free\n  approval: instant, email-verified\n  note: >-\n    The key is an api.data.gov key, not an FTC-issued credential — the same key works\n    against every api.data.gov-fronted federal API.\ntransport:\n  https_required: true\n  http_behavior: HTTP requests are rejected with HTTP 400 / HTTPS_REQUIRED\n  source: https://www.ftc.gov/developer/api/v0/endpoints/hsr-early-termination-notices\noauth: false\nopenid_connect: false\nmtls: false\nscopes: false\nscopes_note: >-\n  No scope surface exists. The API is read-only and a key carries no per-resource\n  permissions, so scopes/ is deliberately absent for this provider.\ngated_surfaces:\n  - name: National\
  \ Do Not Call Registry (telemarketer access)\n    url: https://telemarketing.donotcall.gov\n    auth: account registration + annual fee, provisioned by the FTC contractor\n    public_contract: false\n  - name: Consumer Sentinel Network\n    url: https://www.ftc.gov/enforcement/consumer-sentinel-network\n    auth: vetted law-enforcement membership\n    public_contract: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-trade-commission/refs/heads/main/authentication/federal-trade-commission-authentication.yml
summary_line: 3 schemes
tags:
- Antitrust
- Consumer Protection
- Do Not Call
- Federal-Government
- Law Enforcement
- Open Data
---
