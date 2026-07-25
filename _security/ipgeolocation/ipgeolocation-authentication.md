---
api_key_in:
- query
api_specs:
- filename: ipgeolocation-asn-lookup-api-openapi.yml
  format: yaml
  label: IPGeolocation.io ASN Lookup API
  slug: ipgeolocation-asn-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-asn-lookup-api-openapi.yml
- filename: ipgeolocation-astronomy-api-openapi.yml
  format: yaml
  label: IPGeolocation.io Astronomy API
  slug: ipgeolocation-astronomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-astronomy-api-openapi.yml
- filename: ipgeolocation-ip-abuse-contact-api-openapi.yml
  format: yaml
  label: IPGeolocation.io IP Abuse Contact API
  slug: ipgeolocation-ip-abuse-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-ip-abuse-contact-api-openapi.yml
- filename: ipgeolocation-ip-geolocation-api-openapi.yml
  format: yaml
  label: IPGeolocation.io IP Geolocation API
  slug: ipgeolocation-ip-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-ip-geolocation-api-openapi.yml
- filename: ipgeolocation-ip-security-api-openapi.yml
  format: yaml
  label: IPGeolocation.io IP Security API
  slug: ipgeolocation-ip-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-ip-security-api-openapi.yml
- filename: ipgeolocation-timezone-api-openapi.yml
  format: yaml
  label: IPGeolocation.io Timezone API
  slug: ipgeolocation-timezone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-timezone-api-openapi.yml
- filename: ipgeolocation-user-agent-api-openapi.yml
  format: yaml
  label: IPGeolocation.io User Agent API
  slug: ipgeolocation-user-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/openapi/ipgeolocation-user-agent-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ipgeolocation Authentication
name_suffix: Authentication
oauth_flows: []
overview: IPGeolocation.io secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IPGeolocation.io
provider_slug: ipgeolocation
scheme_count: 1
schemes:
- description: 'API key passed as the `apiKey` query parameter. Get yours from the

    [IPGeolocation dashboard](https://app.ipgeolocation.io/). For client-side

    usage, consider using Request Origin (CORS) authentication instead to

    avoid exposing your key.'
  in: query
  name: ApiKeyAuth
  parameter: apiKey
  sources:
  - openapi/ipgeolocation-abuse-openapi.yml
  - openapi/ipgeolocation-asn-openapi.yml
  - openapi/ipgeolocation-astronomy-openapi.yml
  - openapi/ipgeolocation-ip-location-openapi.yml
  - openapi/ipgeolocation-security-openapi.yml
  - openapi/ipgeolocation-timezone-openapi.yml
  - openapi/ipgeolocation-user-agent-openapi.yml
  type: apiKey
slug: ipgeolocation-authentication
source_filename: ipgeolocation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ipgeolocation-abuse-openapi.yml, openapi/ipgeolocation-asn-openapi.yml, openapi/ipgeolocation-astronomy-openapi.yml,\n  openapi/ipgeolocation-ip-location-openapi.yml, openapi/ipgeolocation-security-openapi.yml,\n  openapi/ipgeolocation-timezone-openapi.yml, openapi/ipgeolocation-user-agent-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: |-\n    API key passed as the `apiKey` query parameter. Get yours from the\n    [IPGeolocation dashboard](https://app.ipgeolocation.io/). For client-side\n    usage, consider using Request Origin (CORS) authentication instead to\n    avoid exposing your key.\n  sources:\n  - openapi/ipgeolocation-abuse-openapi.yml\n  - openapi/ipgeolocation-asn-openapi.yml\n  - openapi/ipgeolocation-astronomy-openapi.yml\n  - openapi/ipgeolocation-ip-location-openapi.yml\n  - openapi/ipgeolocation-security-openapi.yml\n\
  \  - openapi/ipgeolocation-timezone-openapi.yml\n  - openapi/ipgeolocation-user-agent-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipgeolocation/refs/heads/main/authentication/ipgeolocation-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Geocoding
- IP Geolocation
- IP Intelligence
- IP Security
- ASN Lookup
- Abuse Contact
- Timezone
- Astronomy
- User Agent
- Threat Intelligence
- Public APIs
---
