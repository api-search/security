---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Insperity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Insperity secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Insperity
provider_slug: insperity
scheme_count: 1
schemes:
- description: The provider states "Currently there is only one way to authenticate through Insperity API." The key is issued by an Insperity Integration Specialist over secure email after an API Terms of Use Agreement is signed; it is not self-service.
  example_request: 'curl -H ''Authorization: APIKey YourApiKey'' ''https://api.insperity.com/public/employee/addresschange/v1'''
  in: header
  name: InsperityAPIKey
  parameter_name: Authorization
  sources:
  - https://developer.insperity.com/developer-resources
  type: apiKey
  value_format: APIKey <YourApiKey>
slug: insperity-authentication
source_filename: insperity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: https://developer.insperity.com/developer-resources\ndocs: https://developer.insperity.com/developer-resources\nnote: >-\n  Insperity publishes no OpenAPI to an anonymous client (the portal's Swagger endpoint,\n  /api/swagger/{category}, returns 401), so this profile is read from the provider's own\n  Developer Resources page rather than derived from a securityScheme block.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  network_controls: [ip-allowlist]\nschemes:\n  - name: InsperityAPIKey\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    value_format: 'APIKey <YourApiKey>'\n    example_request: \"curl -H 'Authorization: APIKey YourApiKey' 'https://api.insperity.com/public/employee/addresschange/v1'\"\n    sources: [https://developer.insperity.com/developer-resources]\n    description: >-\n      The provider states \"Currently there is only one way to authenticate through\
  \ Insperity API.\"\n      The key is issued by an Insperity Integration Specialist over secure email after an API Terms of\n      Use Agreement is signed; it is not self-service.\nissuance:\n  self_service: false\n  process: >-\n    Sign the API Terms of Use Agreement, provide Insperity client IDs, provide the IP addresses or\n    IP range to be allow-listed, then an Insperity Integration Specialist creates the API Connection\n    and sends the key by secure email. A separate production key/URL pair is issued after stage testing.\n  contact: https://developer.insperity.com/get-started\nrotation:\n  expiry: annual\n  evidence: 'Get Started page: \"Keys expire annually.\"'\n  source: https://developer.insperity.com/get-started\nnetwork_controls:\n  ip_allowlisting:\n    required: true\n    evidence: >-\n      \"Due to the sensitive nature of the data, we only allow connections from approved IP addresses.\n      A list of IP addresses or ranges must be provided to your Integration Specialist.\"\
  \n    source: https://developer.insperity.com/get-started\ntenancy:\n  client_id_required: true\n  note: >-\n    Every request must carry an Insperity client ID; a request missing it is rejected, and a target\n    client ID not enabled for the presented key returns 403.\nauth_failure_semantics:\n  note: >-\n    \"Authentication requests can return either 404 Not Found or 403 Forbidden depending on the\n    situation. This is to prevent the accidental release of sensitive information to unauthorized users.\"\n  statuses: [401, 403, 404]\noauth: false\nopenid_connect: false\nmutual_tls: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insperity/refs/heads/main/authentication/insperity-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Fortune 1000
- Human Resources
- Payroll
- Benefits
- HRIS
- Onboarding
- Professional Employer Organization
- Workforce Management
- Employer of Record
---
