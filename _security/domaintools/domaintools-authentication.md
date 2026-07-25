---
api_key_in:
- header
- query
api_specs:
- filename: domaintools-flex-search-api-openapi.yml
  format: yaml
  label: DomainTools Flex search API
  slug: domaintools-flex-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-flex-search-api-openapi.yml
- filename: domaintools-information-api-openapi.yml
  format: yaml
  label: DomainTools Information API
  slug: domaintools-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-information-api-openapi.yml
- filename: domaintools-iris-detect-api-openapi.yml
  format: yaml
  label: DomainTools Iris Detect API
  slug: domaintools-iris-detect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-iris-detect-api-openapi.yml
- filename: domaintools-iris-enrich-api-openapi.yml
  format: yaml
  label: DomainTools Iris Enrich API
  slug: domaintools-iris-enrich-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-iris-enrich-api-openapi.yml
- filename: domaintools-iris-investigate-api-openapi.yml
  format: yaml
  label: DomainTools Iris Investigate API
  slug: domaintools-iris-investigate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-iris-investigate-api-openapi.yml
- filename: domaintools-lookups-api-openapi.yml
  format: yaml
  label: DomainTools Lookups API
  slug: domaintools-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-lookups-api-openapi.yml
- filename: domaintools-monitors-api-openapi.yml
  format: yaml
  label: DomainTools Monitors API
  slug: domaintools-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-monitors-api-openapi.yml
- filename: domaintools-ping-api-openapi.yml
  format: yaml
  label: DomainTools Ping API
  slug: domaintools-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-ping-api-openapi.yml
- filename: domaintools-rate-limit-api-openapi.yml
  format: yaml
  label: DomainTools Rate Limit API
  slug: domaintools-rate-limit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-rate-limit-api-openapi.yml
- filename: domaintools-rdata-lookups-api-openapi.yml
  format: yaml
  label: DomainTools rdata Lookups API
  slug: domaintools-rdata-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-rdata-lookups-api-openapi.yml
- filename: domaintools-rrset-lookups-api-openapi.yml
  format: yaml
  label: DomainTools rrset Lookups API
  slug: domaintools-rrset-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-rrset-lookups-api-openapi.yml
- filename: domaintools-siebatchd-api-openapi.yml
  format: yaml
  label: DomainTools Siebatchd API
  slug: domaintools-siebatchd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/openapi/domaintools-siebatchd-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Domaintools Authentication
name_suffix: Authentication
oauth_flows: []
overview: DomainTools secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DomainTools
provider_slug: domaintools
scheme_count: 4
schemes:
- in: header
  name: apikey
  parameter: X-API-KEY
  sources:
  - openapi/domaintools-dnsdb-openapi.yml
  type: apiKey
- description: A secure authentication method where the API key is provided in the `X-Api-Key` HTTP request header.
  in: header
  name: header_auth
  parameter: X-Api-Key
  sources:
  - openapi/domaintools-iris-openapi.yml
  - openapi/domaintools-lookups-monitors-openapi.yml
  type: apiKey
- description: A simple authentication scheme using your `api_username` as the username and your `api_key` as the password. We strongly recommend using HMAC or Header authentication instead to avoid exposing your credentials.
  name: open_key_auth
  scheme: basic
  sources:
  - openapi/domaintools-iris-openapi.yml
  - openapi/domaintools-lookups-monitors-openapi.yml
  type: http
- description: 'A secure scheme using a Hashed Message Authentication Code (HMAC).

    This method requires three query parameters to be sent with the request:

    1. `api_username`: Your API username.

    2. `timestamp`: The current timestamp in ISO 8601 format (e.g., `2020-02-01T22:37:59Z`).

    3. `signature`: The HMAC signature of the request. This is a hash (SHA-256 recommended) of your username, the timestamp, and the requ'
  in: query
  name: hmac_auth
  parameter: signature
  sources:
  - openapi/domaintools-iris-openapi.yml
  - openapi/domaintools-lookups-monitors-openapi.yml
  type: apiKey
slug: domaintools-authentication
source_filename: domaintools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/domaintools-dnsdb-openapi.yml, openapi/domaintools-iris-openapi.yml, openapi/domaintools-lookups-monitors-openapi.yml\ndocs: https://docs.domaintools.com/authentication/\nnotes: >-\n  Docs confirm three credential styles: X-Api-Key header (recommended default),\n  HMAC request signing (recommended for production — the api key never travels\n  over the wire), and http basic (api_username + api_key, discouraged). Query-\n  string api key is supported for Iris/Lookups/Threat Feeds but discouraged.\n  Farsight SIE Batch uniquely takes the api key as an `apikey` field in the JSON\n  POST body. No OAuth token flow is documented for the core product APIs.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/domaintools-dnsdb-openapi.yml\n- name: header_auth\n  type: apiKey\n  in: header\n  parameter:\
  \ X-Api-Key\n  description: A secure authentication method where the API key is provided in the `X-Api-Key`\n    HTTP request header.\n  sources:\n  - openapi/domaintools-iris-openapi.yml\n  - openapi/domaintools-lookups-monitors-openapi.yml\n- name: open_key_auth\n  type: http\n  scheme: basic\n  description: A simple authentication scheme using your `api_username` as the username and\n    your `api_key` as the password. We strongly recommend using HMAC or Header authentication\n    instead to avoid exposing your credentials.\n  sources:\n  - openapi/domaintools-iris-openapi.yml\n  - openapi/domaintools-lookups-monitors-openapi.yml\n- name: hmac_auth\n  type: apiKey\n  in: query\n  parameter: signature\n  description: |-\n    A secure scheme using a Hashed Message Authentication Code (HMAC).\n    This method requires three query parameters to be sent with the request:\n    1. `api_username`: Your API username.\n    2. `timestamp`: The current timestamp in ISO 8601 format (e.g., `2020-02-01T22:37:59Z`).\n\
  \    3. `signature`: The HMAC signature of the request. This is a hash (SHA-256 recommended) of your username, the timestamp, and the requ\n  sources:\n  - openapi/domaintools-iris-openapi.yml\n  - openapi/domaintools-lookups-monitors-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/domaintools/refs/heads/main/authentication/domaintools-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- Company
- Threat Intelligence
- Domain Intelligence
- DNS
- WHOIS
- Passive DNS
- Cybersecurity
- Domain Monitoring
- Risk Scoring
- Security
---
