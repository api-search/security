---
api_key_in:
- header
api_specs:
- filename: spycloud-breach-api-openapi.yml
  format: yaml
  label: SpyCloud Breach API
  slug: spycloud-breach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/openapi/spycloud-breach-api-openapi.yml
- filename: spycloud-check-api-openapi.yml
  format: yaml
  label: SpyCloud Check API
  slug: spycloud-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/openapi/spycloud-check-api-openapi.yml
- filename: spycloud-compass-api-openapi.yml
  format: yaml
  label: SpyCloud Compass API
  slug: spycloud-compass-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/openapi/spycloud-compass-api-openapi.yml
- filename: spycloud-data-api-openapi.yml
  format: yaml
  label: SpyCloud Data API
  slug: spycloud-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/openapi/spycloud-data-api-openapi.yml
- filename: spycloud-query-api-openapi.yml
  format: yaml
  label: SpyCloud Query API
  slug: spycloud-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/openapi/spycloud-query-api-openapi.yml
- filename: spycloud-stats-api-openapi.yml
  format: yaml
  label: SpyCloud Stats API
  slug: spycloud-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/openapi/spycloud-stats-api-openapi.yml
- filename: spycloud-watchlist-api-openapi.yml
  format: yaml
  label: SpyCloud Watchlist API
  slug: spycloud-watchlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/openapi/spycloud-watchlist-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Spycloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpyCloud secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SpyCloud
provider_slug: spycloud
scheme_count: 2
schemes:
- in: header
  name: sec0
  parameter: x-api-key
  sources:
  - openapi/spycloud-compromised-credit-card-openapi.yml
  - openapi/spycloud-consumer-ato-prevention-openapi.yml
  - openapi/spycloud-data-partnership-openapi.yml
  - openapi/spycloud-idlink-openapi.yml
  - openapi/spycloud-investigations-openapi.yml
  - openapi/spycloud-nist-password-openapi.yml
  - openapi/spycloud-prospecting-openapi.yml
  - openapi/spycloud-session-identity-protection-openapi.yml
  type: apiKey
- in: header
  name: sec0
  parameter: X-API-KEY
  sources:
  - openapi/spycloud-enterprise-ato-prevention-openapi.yml
  type: apiKey
slug: spycloud-authentication
source_filename: spycloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: openapi/spycloud-compromised-credit-card-openapi.yml, openapi/spycloud-consumer-ato-prevention-openapi.yml,\n  openapi/spycloud-data-partnership-openapi.yml, openapi/spycloud-enterprise-ato-prevention-openapi.yml, openapi/spycloud-idlink-openapi.yml,\n  openapi/spycloud-investigations-openapi.yml, openapi/spycloud-nist-password-openapi.yml, openapi/spycloud-prospecting-openapi.yml,\n  openapi/spycloud-session-identity-protection-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  header_names:\n  - x-api-key\n  - X-API-KEY\n  oauth2: false\n  note: Single-scheme API-key auth across all nine SpyCloud APIs. There is no OAuth 2.0 / OIDC surface, so no scopes/\n    artifact is emitted.\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/spycloud-compromised-credit-card-openapi.yml\n  - openapi/spycloud-consumer-ato-prevention-openapi.yml\n  - openapi/spycloud-data-partnership-openapi.yml\n\
  \  - openapi/spycloud-idlink-openapi.yml\n  - openapi/spycloud-investigations-openapi.yml\n  - openapi/spycloud-nist-password-openapi.yml\n  - openapi/spycloud-prospecting-openapi.yml\n  - openapi/spycloud-session-identity-protection-openapi.yml\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/spycloud-enterprise-ato-prevention-openapi.yml\ndocs: https://docs.spycloud.com/public-sc/docs/api-guidelines\nkey_management:\n  issued_via: https://portal.spycloud.com\n  console_page: https://docs.spycloud.com/public-sc/docs/account-settings\n  note: API keys are created and rotated in the SpyCloud Customer Portal; keys carry broad privileges and must not\n    be embedded in client-side code or repositories.\ncontrols:\n- control: transport\n  detail: All requests must be HTTPS. TLS 1.2 and TLS 1.3 supported; TLS 1.3 ciphers TLS_AES_128_GCM_SHA256, TLS_AES_256_GCM_SHA384,\n    TLS_CHACHA20_POLY1305_SHA256.\n- control: ip-allow-list\n  detail: Access\
  \ is restricted to a customer-supplied list of IPv4 addresses or CIDRs. Calls from a non-allow-listed\n    IP return HTTP 403.\n- control: api-function-allow-list\n  detail: A key is entitled to all or a contract-defined subset of API functions. Calling an unentitled function\n    returns HTTP 403.\n- control: asset-allow-list\n  detail: Response fields can be restricted per key; non-allow-listed assets are masked with a fixed 8-asterisk\n    string. document_id, source_id and spycloud_publish_date are always returned.\n- control: asset-hashing\n  detail: Optionally returns salted hashes instead of plaintext assets. Algorithms sha1, sha224, sha256, sha384,\n    sha512; 10-24 character high-entropy salt, positioned right by default, overridable per call via the salt query\n    parameter.\n- control: cors\n  detail: CORS is supported for browser clients, though SpyCloud warns against exposing API keys in public client-side\n    code.\nfailure_modes:\n- status: 403\n  meaning: Missing/invalid\
  \ key, non-allow-listed source IP, or an endpoint the key is not entitled to.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spycloud/refs/heads/main/authentication/spycloud-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Cybersecurity
- Threat Intelligence
- Identity
- Fraud Prevention
- Account Takeover
- Dark Web
- Breach Data
- Malware
- Authentication
- Security
---
