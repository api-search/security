---
api_key_in: []
api_specs:
- filename: cisco-expressway-admin-account-api-openapi.yml
  format: yaml
  label: Cisco Expressway Admin Account API
  slug: cisco-expressway-admin-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-admin-account-api-openapi.yml
- filename: cisco-expressway-alarms-api-openapi.yml
  format: yaml
  label: Cisco Expressway Alarms API
  slug: cisco-expressway-alarms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-alarms-api-openapi.yml
- filename: cisco-expressway-calls-api-openapi.yml
  format: yaml
  label: Cisco Expressway Calls API
  slug: cisco-expressway-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-calls-api-openapi.yml
- filename: cisco-expressway-dns-api-openapi.yml
  format: yaml
  label: Cisco Expressway DNS API
  slug: cisco-expressway-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-dns-api-openapi.yml
- filename: cisco-expressway-licensing-api-openapi.yml
  format: yaml
  label: Cisco Expressway Licensing API
  slug: cisco-expressway-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-licensing-api-openapi.yml
- filename: cisco-expressway-ntp-api-openapi.yml
  format: yaml
  label: Cisco Expressway NTP API
  slug: cisco-expressway-ntp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-ntp-api-openapi.yml
- filename: cisco-expressway-registrations-api-openapi.yml
  format: yaml
  label: Cisco Expressway Registrations API
  slug: cisco-expressway-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-registrations-api-openapi.yml
- filename: cisco-expressway-resource-usage-api-openapi.yml
  format: yaml
  label: Cisco Expressway Resource Usage API
  slug: cisco-expressway-resource-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-resource-usage-api-openapi.yml
- filename: cisco-expressway-search-rules-api-openapi.yml
  format: yaml
  label: Cisco Expressway Search Rules API
  slug: cisco-expressway-search-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-search-rules-api-openapi.yml
- filename: cisco-expressway-sftp-api-openapi.yml
  format: yaml
  label: Cisco Expressway SFTP API
  slug: cisco-expressway-sftp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-sftp-api-openapi.yml
- filename: cisco-expressway-sip-api-openapi.yml
  format: yaml
  label: Cisco Expressway SIP API
  slug: cisco-expressway-sip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-sip-api-openapi.yml
- filename: cisco-expressway-system-api-openapi.yml
  format: yaml
  label: Cisco Expressway System API
  slug: cisco-expressway-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-system-api-openapi.yml
- filename: cisco-expressway-system-status-api-openapi.yml
  format: yaml
  label: Cisco Expressway System Status API
  slug: cisco-expressway-system-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-system-status-api-openapi.yml
- filename: cisco-expressway-transforms-api-openapi.yml
  format: yaml
  label: Cisco Expressway Transforms API
  slug: cisco-expressway-transforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-transforms-api-openapi.yml
- filename: cisco-expressway-upgrade-api-openapi.yml
  format: yaml
  label: Cisco Expressway Upgrade API
  slug: cisco-expressway-upgrade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-upgrade-api-openapi.yml
- filename: cisco-expressway-zones-api-openapi.yml
  format: yaml
  label: Cisco Expressway Zones API
  slug: cisco-expressway-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/openapi/cisco-expressway-zones-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cisco Expressway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Expressway secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cisco Expressway
provider_slug: cisco-expressway
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using Expressway administrator credentials. The API is only accessible via HTTPS.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/cisco-expressway-configuration-api-openapi.yml
  - openapi/cisco-expressway-status-api-openapi.yml
  type: http
slug: cisco-expressway-authentication
source_filename: cisco-expressway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-expressway-configuration-api-openapi.yml, openapi/cisco-expressway-status-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using Expressway administrator credentials. The API\n    is only accessible via HTTPS.\n  sources:\n  - openapi/cisco-expressway-configuration-api-openapi.yml\n  - openapi/cisco-expressway-status-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-expressway/refs/heads/main/authentication/cisco-expressway-authentication.yml
summary_line: http · 1 scheme
tags:
- Collaboration
- Firewall Traversal
- H.323
- Session Border Controller
- SIP
- Unified Communications
- Video Conferencing
---
