---
api_key_in:
- query
api_specs:
- filename: ipinfo-abuse-api-openapi.yml
  format: yaml
  label: IPinfo abuse API
  slug: ipinfo-abuse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-abuse-api-openapi.yml
- filename: ipinfo-asn-api-openapi.yml
  format: yaml
  label: IPinfo asn API
  slug: ipinfo-asn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-asn-api-openapi.yml
- filename: ipinfo-carrier-api-openapi.yml
  format: yaml
  label: IPinfo carrier API
  slug: ipinfo-carrier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-carrier-api-openapi.yml
- filename: ipinfo-company-api-openapi.yml
  format: yaml
  label: IPinfo company API
  slug: ipinfo-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-company-api-openapi.yml
- filename: ipinfo-domains-api-openapi.yml
  format: yaml
  label: IPinfo domains API
  slug: ipinfo-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-domains-api-openapi.yml
- filename: ipinfo-general-api-openapi.yml
  format: yaml
  label: IPinfo general API
  slug: ipinfo-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-general-api-openapi.yml
- filename: ipinfo-ipinfo-core-api-openapi.yml
  format: yaml
  label: IPinfo ipinfo core API
  slug: ipinfo-ipinfo-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-ipinfo-core-api-openapi.yml
- filename: ipinfo-ipinfo-lite-api-openapi.yml
  format: yaml
  label: IPinfo ipinfo lite API
  slug: ipinfo-ipinfo-lite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-ipinfo-lite-api-openapi.yml
- filename: ipinfo-ipinfo-max-api-openapi.yml
  format: yaml
  label: IPinfo ipinfo max API
  slug: ipinfo-ipinfo-max-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-ipinfo-max-api-openapi.yml
- filename: ipinfo-ipinfo-plus-api-openapi.yml
  format: yaml
  label: IPinfo ipinfo plus API
  slug: ipinfo-ipinfo-plus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-ipinfo-plus-api-openapi.yml
- filename: ipinfo-places-api-openapi.yml
  format: yaml
  label: IPinfo places API
  slug: ipinfo-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-places-api-openapi.yml
- filename: ipinfo-privacy-detection-api-openapi.yml
  format: yaml
  label: IPinfo privacy detection API
  slug: ipinfo-privacy-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-privacy-detection-api-openapi.yml
- filename: ipinfo-privacy-detection-extended-api-openapi.yml
  format: yaml
  label: IPinfo privacy detection extended API
  slug: ipinfo-privacy-detection-extended-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-privacy-detection-extended-api-openapi.yml
- filename: ipinfo-ranges-api-openapi.yml
  format: yaml
  label: IPinfo ranges API
  slug: ipinfo-ranges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-ranges-api-openapi.yml
- filename: ipinfo-residential-proxy-detection-api-openapi.yml
  format: yaml
  label: IPinfo residential proxy detection API
  slug: ipinfo-residential-proxy-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-residential-proxy-detection-api-openapi.yml
- filename: ipinfo-single-api-openapi.yml
  format: yaml
  label: IPinfo single API
  slug: ipinfo-single-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-single-api-openapi.yml
- filename: ipinfo-whois-api-openapi.yml
  format: yaml
  label: IPinfo whois API
  slug: ipinfo-whois-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/openapi/ipinfo-whois-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Ipinfo Authentication
name_suffix: Authentication
oauth_flows: []
overview: IPinfo secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: IPinfo
provider_slug: ipinfo
scheme_count: 3
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/ipinfo-openapi.yml
  type: http
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ipinfo-openapi.yml
  type: http
- in: query
  name: ApiKeyAuth
  parameter: token
  sources:
  - openapi/ipinfo-openapi.yml
  type: apiKey
slug: ipinfo-authentication
source_filename: ipinfo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nsource: openapi/ipinfo-openapi.yml\ndocs: https://ipinfo.io/developers#authentication\nnote: >-\n  IPinfo uses a single access token accepted three ways, all documented: HTTP\n  Basic Auth (token as username, empty password), Bearer token in the\n  Authorization header, and a ?token= query parameter. There is no OAuth or\n  scope system.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/ipinfo-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ipinfo-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: token\n  sources:\n  - openapi/ipinfo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/authentication/ipinfo-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- IP Intelligence
- IP Geolocation
- ASN
- Privacy Detection
- VPN Detection
- Threat Intelligence
- Network Data
- Mobile Carrier
- WHOIS
- Public APIs
- Development
---
