---
api_key_in: []
api_specs:
- filename: london-stock-exchange-group-case-api-openapi.yml
  format: yaml
  label: LSEG World-Check One Case API
  slug: lseg-world-check-one-case-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/london-stock-exchange-group-case-api-openapi.yml
- filename: london-stock-exchange-group-media-check-api-openapi.yml
  format: yaml
  label: LSEG World-Check One Media-Check API
  slug: lseg-world-check-one-media-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/london-stock-exchange-group-media-check-api-openapi.yml
- filename: london-stock-exchange-group-smart-filter-api-openapi.yml
  format: yaml
  label: LSEG World-Check One Smart Filter API
  slug: lseg-world-check-one-smart-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/london-stock-exchange-group-smart-filter-api-openapi.yml
- filename: london-stock-exchange-group-audit-api-openapi.yml
  format: yaml
  label: LSEG World-Check One Audit API
  slug: lseg-world-check-one-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/london-stock-exchange-group-audit-api-openapi.yml
- filename: london-stock-exchange-group-case-rating-api-openapi.yml
  format: yaml
  label: LSEG World-Check One Case Rating API
  slug: lseg-world-check-one-case-rating-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/london-stock-exchange-group-case-rating-api-openapi.yml
- filename: london-stock-exchange-group-linked-cases-api-openapi.yml
  format: yaml
  label: LSEG World-Check One Linked Cases API
  slug: lseg-world-check-one-linked-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/london-stock-exchange-group-linked-cases-api-openapi.yml
- filename: london-stock-exchange-group-group-api-openapi.yml
  format: yaml
  label: LSEG World-Check One Group API
  slug: lseg-world-check-one-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/london-stock-exchange-group-group-api-openapi.yml
- filename: london-stock-exchange-group-user-api-openapi.yml
  format: yaml
  label: LSEG World-Check One User API
  slug: lseg-world-check-one-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/london-stock-exchange-group-user-api-openapi.yml
- filename: london-stock-exchange-group-reference-api-openapi.yml
  format: yaml
  label: LSEG World-Check One Reference API
  slug: lseg-world-check-one-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/london-stock-exchange-group-reference-api-openapi.yml
- filename: london-stock-exchange-group-client-watchlist-api-openapi.yml
  format: yaml
  label: LSEG World-Check One Client Watchlist API
  slug: lseg-world-check-one-client-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/london-stock-exchange-group-client-watchlist-api-openapi.yml
- filename: london-stock-exchange-group-reporting-api-openapi.yml
  format: yaml
  label: LSEG World-Check One Reporting API
  slug: lseg-world-check-one-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/london-stock-exchange-group-reporting-api-openapi.yml
- filename: london-stock-exchange-group-upcoming-api-openapi.yml
  format: yaml
  label: LSEG World-Check One Upcoming API
  slug: lseg-world-check-one-upcoming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/london-stock-exchange-group-upcoming-api-openapi.yml
- filename: london-stock-exchange-group-passport-check-api-openapi.yml
  format: yaml
  label: LSEG World-Check One Passport Check API
  slug: lseg-world-check-one-passport-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/london-stock-exchange-group-passport-check-api-openapi.yml
- filename: london-stock-exchange-group-zfs-api-openapi.yml
  format: yaml
  label: LSEG World-Check One Zero Footprint Screening API
  slug: lseg-world-check-one-zfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/london-stock-exchange-group-zfs-api-openapi.yml
- filename: london-stock-exchange-group-api-info-api-openapi.yml
  format: yaml
  label: LSEG World-Check One API Info API
  slug: lseg-world-check-one-api-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/openapi/london-stock-exchange-group-api-info-api-openapi.yml
auth_types:
- oauth2
- hmac-signature
description: ''
kind: authentication
layout: security
method: searched
name: London Stock Exchange Group Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: London Stock Exchange Group secures its APIs with oauth2 and hmac-signature across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: London Stock Exchange Group
provider_slug: london-stock-exchange-group
scheme_count: 2
schemes:
- applies_to: v3 (https://api.risk.lseg.com/screening/v3/)
  description: 'Recommended for API v3. A service account is provisioned in the World-Check One admin portal (requires the Service Account Admin role): service-account-uuid acts as the client ID and service-account-password as the client secret.'
  flow: clientCredentials
  name: oauth2ServiceAccount
  type: oauth2
- algorithm: hmac-sha256
  applies_to: v2 (https://api-worldcheck.refinitiv.com/v2) and v3
  authorization_header: 'Authorization: Signature keyId="{API-KEY}",algorithm="hmac-sha256", headers="(request-target) host date content-type content-length", signature="{BASE64-HMAC-VALUE}"'
  description: Every request is signed with a keyed-hash message authentication code. Each API user is issued an API key (public identifier, UUID format) and an 88-character symmetric API secret known only to the user and the World-Check One system; the secret is never transmitted. The signature covers the request target, host, date, content-type and content-length, and requests are replay-protected by validating the Date header (RFC 1123 format) against the processing time.
  name: hmacSignature
  required_headers:
  - Authorization
  - Date
  type: http-signature
slug: london-stock-exchange-group-authentication
source_filename: london-stock-exchange-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\ndocs: https://developers.lseg.com/en/api-catalog/customer-and-third-party-screening/world-check-one-api/quick-start\nsource: >-\n  World-Check One API quick start + security documentation (the OpenAPI 2.0\n  definition declares no securityDefinitions; the auth contract is documented\n  in the developer portal, so this profile is searched, not derived)\nsummary:\n  types: [oauth2, hmac-signature]\n  oauth2_flows: [clientCredentials]\n  notes: >-\n    API v3 (api.risk.lseg.com/screening/v3/) recommends OAuth 2.0\n    service-account credentials; API v2 (api-worldcheck.refinitiv.com/v2) uses\n    per-user API key + HMAC-SHA256 signed requests.\nschemes:\n  - name: oauth2ServiceAccount\n    type: oauth2\n    flow: clientCredentials\n    description: >-\n      Recommended for API v3. A service account is provisioned in the\n      World-Check One admin portal (requires the Service Account Admin role):\n      service-account-uuid acts as\
  \ the client ID and service-account-password\n      as the client secret.\n    applies_to: v3 (https://api.risk.lseg.com/screening/v3/)\n  - name: hmacSignature\n    type: http-signature\n    algorithm: hmac-sha256\n    description: >-\n      Every request is signed with a keyed-hash message authentication code.\n      Each API user is issued an API key (public identifier, UUID format) and\n      an 88-character symmetric API secret known only to the user and the\n      World-Check One system; the secret is never transmitted. The signature\n      covers the request target, host, date, content-type and content-length,\n      and requests are replay-protected by validating the Date header\n      (RFC 1123 format) against the processing time.\n    authorization_header: >-\n      Authorization: Signature keyId=\"{API-KEY}\",algorithm=\"hmac-sha256\",\n      headers=\"(request-target) host date content-type content-length\",\n      signature=\"{BASE64-HMAC-VALUE}\"\n    required_headers: [Authorization,\
  \ Date]\n    applies_to: v2 (https://api-worldcheck.refinitiv.com/v2) and v3\ncredentials:\n  - name: API key\n    kind: public identifier\n    format: 8-4-4-4-12 character UUID\n  - name: API secret\n    kind: symmetric secret\n    format: 88 characters\n  - name: service-account-uuid / service-account-password\n    kind: OAuth 2.0 client credentials (v3)\nnotes: >-\n  Credentials are issued per environment (Pilot vs Production) by the LSEG\n  account team; there is no self-service sign-up. See\n  sandbox/london-stock-exchange-group-sandbox.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/london-stock-exchange-group/refs/heads/main/authentication/london-stock-exchange-group-authentication.yml
summary_line: oauth2/hmac-signature · 2 schemes
tags:
- Financial
- Stock Exchange
- Market Data
- KYC
- Compliance
---
