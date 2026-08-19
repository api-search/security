---
api_key_in:
- header
- cookie
api_specs:
- filename: cisco-catalyst-sdwan-administration-and-settings-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Administration and Settings
  slug: administration-and-settings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-administration-and-settings-openapi.json
- filename: cisco-catalyst-sdwan-ux-1-0-configuration-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — UX 1.0 Configuration
  slug: ux-1-0-configuration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-ux-1-0-configuration-openapi.json
- filename: cisco-catalyst-sdwan-ux-2-0-configuration-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — UX 2.0 Configuration
  slug: ux-2-0-configuration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-ux-2-0-configuration-openapi.json
- filename: cisco-catalyst-sdwan-feature-profiles-sd-wan-system-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Feature Profiles - SD-WAN System
  slug: feature-profiles-sd-wan-system
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-feature-profiles-sd-wan-system-openapi.json
- filename: cisco-catalyst-sdwan-feature-profiles-sd-wan-transport-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Feature Profiles - SD-WAN Transport
  slug: feature-profiles-sd-wan-transport
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-feature-profiles-sd-wan-transport-openapi.json
- filename: cisco-catalyst-sdwan-feature-profiles-sd-wan-service-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Feature Profiles - SD-WAN Service
  slug: feature-profiles-sd-wan-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-feature-profiles-sd-wan-service-openapi.json
- filename: cisco-catalyst-sdwan-feature-profiles-others-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Feature Profiles - Others
  slug: feature-profiles-others
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-feature-profiles-others-openapi.json
- filename: cisco-catalyst-sdwan-feature-profiles-sd-routing-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Feature Profiles - SD-Routing
  slug: feature-profiles-sd-routing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-feature-profiles-sd-routing-openapi.json
- filename: cisco-catalyst-sdwan-feature-profiles-mobility-and-nfv-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Feature Profiles - Mobility and NFV
  slug: feature-profiles-mobility-and-nfv
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-feature-profiles-mobility-and-nfv-openapi.json
- filename: cisco-catalyst-sdwan-monitoring-and-troubleshooting-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Monitoring and Troubleshooting
  slug: monitoring-and-troubleshooting
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-monitoring-and-troubleshooting-openapi.json
- filename: cisco-catalyst-sdwan-sd-wan-services-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — SD-WAN Services
  slug: sd-wan-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-sd-wan-services-openapi.json
- filename: cisco-catalyst-sdwan-partner-integrations-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Partner Integrations
  slug: partner-integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-partner-integrations-openapi.json
- filename: cisco-catalyst-sdwan-others-openapi.json
  format: json
  label: Cisco Catalyst SD-WAN Manager API — Others
  slug: others
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/openapi/cisco-catalyst-sdwan-others-openapi.json
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cisco Catalyst Sdwan Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco Catalyst SD-WAN secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cisco Catalyst SD-WAN
provider_slug: cisco-catalyst-sdwan
scheme_count: 3
schemes:
- bearerFormat: JWT
  login:
    body_fields:
    - username
    - password
    - duration
    content_type: application/json
    default_duration_seconds: 1800
    max_duration_seconds: 604800
    method: POST
    path: /jwt/login
  name: jwtBearer
  refresh:
    note: refresh token returned alongside the access token
    path: /jwt/refresh
  response_claims:
  - token
  - refresh
  - sub
  - iss
  - aud
  - userGroup
  - tenant
  - duration
  - exp
  - csrf
  - isAPIKey
  - tenantId
  scheme: bearer
  since: SD-WAN Manager 20.18.1
  source: https://developer.cisco.com/docs/sdwan/authentication/#jwt-based-authentication
  standard: RFC 7519
  type: http
- in: header
  name: xsrfToken
  note: Cross-site request forgery token required for most POST/PUT/DELETE operations. With JWT it arrives in the "csrf" claim of the login response; with session auth it is fetched from GET /dataservice/client/token.
  parameter: X-XSRF-TOKEN
  source: https://developer.cisco.com/docs/sdwan/authentication/
  type: apiKey
- in: cookie
  legacy: true
  login:
    body_fields:
    - j_username
    - j_password
    content_type: application/x-www-form-urlencoded
    method: POST
    path: /j_security_check
  name: jsessionid
  note: Session-based authentication retained for backward compatibility.
  parameter: JSESSIONID
  source: https://developer.cisco.com/docs/sdwan/authentication/#session-based-authentication
  type: apiKey
slug: cisco-catalyst-sdwan-authentication
source_filename: cisco-catalyst-sdwan-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: searched\nsource: https://developer.cisco.com/docs/sdwan/authentication/\ndocs: https://developer.cisco.com/docs/sdwan/authentication/\nnote: The 13 harvested OpenAPI documents declare NO components.securitySchemes and no operation-level\n  security[] — the authentication model lives only in the DevNet prose docs, not in the machine-readable\n  contract. The login endpoints (POST /jwt/login, POST /j_security_check, GET /dataservice/client/token)\n  are not present in any of the 4,138 harvested operations. This profile is searched from the docs.\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  - cookie\n  oauth2_flows: []\n  spec_declares_security: false\n  documented_only: true\nschemes:\n- name: jwtBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  since: SD-WAN Manager 20.18.1\n  login:\n    method: POST\n    path: /jwt/login\n    content_type: application/json\n    body_fields:\n    - username\n    - password\n\
  \    - duration\n    default_duration_seconds: 1800\n    max_duration_seconds: 604800\n  response_claims:\n  - token\n  - refresh\n  - sub\n  - iss\n  - aud\n  - userGroup\n  - tenant\n  - duration\n  - exp\n  - csrf\n  - isAPIKey\n  - tenantId\n  refresh:\n    path: /jwt/refresh\n    note: refresh token returned alongside the access token\n  standard: RFC 7519\n  source: https://developer.cisco.com/docs/sdwan/authentication/#jwt-based-authentication\n- name: xsrfToken\n  type: apiKey\n  in: header\n  parameter: X-XSRF-TOKEN\n  note: Cross-site request forgery token required for most POST/PUT/DELETE operations. With JWT it arrives\n    in the \"csrf\" claim of the login response; with session auth it is fetched from GET /dataservice/client/token.\n  source: https://developer.cisco.com/docs/sdwan/authentication/\n- name: jsessionid\n  type: apiKey\n  in: cookie\n  parameter: JSESSIONID\n  legacy: true\n  login:\n    method: POST\n    path: /j_security_check\n    content_type: application/x-www-form-urlencoded\n\
  \    body_fields:\n    - j_username\n    - j_password\n  note: Session-based authentication retained for backward compatibility.\n  source: https://developer.cisco.com/docs/sdwan/authentication/#session-based-authentication\napi_keys:\n  supported: true\n  note: A JWT access token issued with isAPIKey=true is a long-lived API key.\nauthorization:\n  model: rbac\n  artifact: scopes/cisco-catalyst-sdwan-scopes.yml\n  note: Every operation carries an x-roles-required extension naming the SD-WAN Manager role(s) needed.\nmultitenancy:\n  supported: true\n  note: JWT carries tenant/tenantId; some APIs are provider-view only.\ntransport:\n  https_required: true\n  default_port: 8443\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-catalyst-sdwan/refs/heads/main/authentication/cisco-catalyst-sdwan-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- SD-WAN
- Networking
- WAN
- Automation
- Policy
- Enterprise
- Network Management
- Infrastructure as Code
- Observability
- Cisco
---
