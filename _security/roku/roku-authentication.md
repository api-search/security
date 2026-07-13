---
api_key_in:
- query
api_specs:
- filename: roku-external-control-protocol.yaml
  format: yaml
  label: Roku External Control Protocol (ECP)
  slug: external-control-protocol
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-external-control-protocol.yaml
- filename: roku-pay-web-services.yaml
  format: yaml
  label: Roku Pay Web Services
  slug: pay
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-pay-web-services.yaml
- filename: roku-nabu-cloud.yaml
  format: yaml
  label: Roku Nabu Cloud
  slug: nabu-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/openapi/roku-nabu-cloud.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Roku Authentication
name_suffix: Authentication
oauth_flows: []
overview: Roku secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Roku
provider_slug: roku
scheme_count: 1
schemes:
- description: 'Roku-issued Partner API Key. For GET endpoints the key is included in the URL path; for

    POST endpoints it is included in the request body. Channels obtain this key from the Roku

    Developer Dashboard.'
  in: query
  name: PartnerAPIKey
  parameter: partnerAPIKey
  sources:
  - openapi/roku-pay-web-services.yaml
  type: apiKey
slug: roku-authentication
source_filename: roku-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/roku-pay-web-services.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: PartnerAPIKey\n  type: apiKey\n  in: query\n  parameter: partnerAPIKey\n  description: |-\n    Roku-issued Partner API Key. For GET endpoints the key is included in the URL path; for\n    POST endpoints it is included in the request body. Channels obtain this key from the Roku\n    Developer Dashboard.\n  sources:\n  - openapi/roku-pay-web-services.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roku/refs/heads/main/authentication/roku-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Streaming
- Television
- Media
- Entertainment
- Connected TV
- Consumer Electronics
---
