---
api_key_in:
- cookie
api_specs:
- filename: cisco-nexus-authentication-api-openapi.yml
  format: yaml
  label: Cisco Nexus Dashboard Authentication API
  slug: cisco-nexus-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/openapi/cisco-nexus-authentication-api-openapi.yml
- filename: cisco-nexus-interfaces-api-openapi.yml
  format: yaml
  label: Cisco Nexus Dashboard Interfaces API
  slug: cisco-nexus-interfaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/openapi/cisco-nexus-interfaces-api-openapi.yml
- filename: cisco-nexus-routing-api-openapi.yml
  format: yaml
  label: Cisco Nexus Dashboard Routing API
  slug: cisco-nexus-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/openapi/cisco-nexus-routing-api-openapi.yml
- filename: cisco-nexus-system-api-openapi.yml
  format: yaml
  label: Cisco Nexus Dashboard System API
  slug: cisco-nexus-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/openapi/cisco-nexus-system-api-openapi.yml
- filename: cisco-nexus-vlans-api-openapi.yml
  format: yaml
  label: Cisco Nexus Dashboard VLANs API
  slug: cisco-nexus-vlans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/openapi/cisco-nexus-vlans-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Cisco Nexus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Nexus Dashboard secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cisco Nexus Dashboard
provider_slug: cisco-nexus
scheme_count: 1
schemes:
- description: Session cookie obtained from the /api/aaaLogin endpoint. The cookie has a configurable idle timeout (default 600 seconds) and must be included in all subsequent requests.
  in: cookie
  name: cookieAuth
  parameter: APIC-cookie
  sources:
  - openapi/cisco-nexus-nxapi-rest.yml
  type: apiKey
slug: cisco-nexus-authentication
source_filename: cisco-nexus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cisco-nexus-nxapi-rest.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: APIC-cookie\n  description: Session cookie obtained from the /api/aaaLogin endpoint. The cookie has a configurable\n    idle timeout (default 600 seconds) and must be included in all subsequent requests.\n  sources:\n  - openapi/cisco-nexus-nxapi-rest.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-nexus/refs/heads/main/authentication/cisco-nexus-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Center
- Infrastructure
- Network Automation
- Networking
- SDN
- Switches
---
