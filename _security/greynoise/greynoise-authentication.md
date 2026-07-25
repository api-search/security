---
api_key_in:
- header
api_specs:
- filename: greynoise-callback-api-openapi.yml
  format: yaml
  label: GreyNoise Intelligence Callback API
  slug: greynoise-callback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greynoise/refs/heads/main/openapi/greynoise-callback-api-openapi.yml
- filename: greynoise-community-api-openapi.yml
  format: yaml
  label: GreyNoise Intelligence Community API
  slug: greynoise-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greynoise/refs/heads/main/openapi/greynoise-community-api-openapi.yml
- filename: greynoise-cve-api-openapi.yml
  format: yaml
  label: GreyNoise Intelligence CVE API
  slug: greynoise-cve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greynoise/refs/heads/main/openapi/greynoise-cve-api-openapi.yml
- filename: greynoise-gnql-api-openapi.yml
  format: yaml
  label: GreyNoise Intelligence GNQL API
  slug: greynoise-gnql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greynoise/refs/heads/main/openapi/greynoise-gnql-api-openapi.yml
- filename: greynoise-ip-lookup-api-openapi.yml
  format: yaml
  label: GreyNoise Intelligence IP Lookup API
  slug: greynoise-ip-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greynoise/refs/heads/main/openapi/greynoise-ip-lookup-api-openapi.yml
- filename: greynoise-ip-timeline-api-openapi.yml
  format: yaml
  label: GreyNoise Intelligence IP Timeline API
  slug: greynoise-ip-timeline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greynoise/refs/heads/main/openapi/greynoise-ip-timeline-api-openapi.yml
- filename: greynoise-recall-api-openapi.yml
  format: yaml
  label: GreyNoise Intelligence Recall API
  slug: greynoise-recall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greynoise/refs/heads/main/openapi/greynoise-recall-api-openapi.yml
- filename: greynoise-sessions-api-openapi.yml
  format: yaml
  label: GreyNoise Intelligence Sessions API
  slug: greynoise-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greynoise/refs/heads/main/openapi/greynoise-sessions-api-openapi.yml
- filename: greynoise-tags-api-openapi.yml
  format: yaml
  label: GreyNoise Intelligence Tags API
  slug: greynoise-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greynoise/refs/heads/main/openapi/greynoise-tags-api-openapi.yml
- filename: greynoise-utility-api-openapi.yml
  format: yaml
  label: GreyNoise Intelligence Utility API
  slug: greynoise-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/greynoise/refs/heads/main/openapi/greynoise-utility-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Greynoise Authentication
name_suffix: Authentication
oauth_flows: []
overview: GreyNoise Intelligence secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GreyNoise Intelligence
provider_slug: greynoise
scheme_count: 1
schemes:
- description: GreyNoise API key passed via the 'key' HTTP header.
  in: header
  name: APIKeyHeaderAuth
  parameter: key
  sources:
  - openapi/greynoise-openapi.yml
  type: apiKey
slug: greynoise-authentication
source_filename: greynoise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/greynoise-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeaderAuth\n  type: apiKey\n  in: header\n  parameter: key\n  description: GreyNoise API key passed via the 'key' HTTP header.\n  sources:\n  - openapi/greynoise-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/greynoise/refs/heads/main/authentication/greynoise-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Security
- Threat Intelligence
- Cybersecurity
- IP Reputation
- Vulnerability Management
- Network Telemetry
- SOC Automation
- Public APIs
---
