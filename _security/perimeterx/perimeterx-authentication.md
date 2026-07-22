---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Perimeterx Authentication
name_suffix: Authentication
oauth_flows: []
overview: PerimeterX (HUMAN Security) secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PerimeterX (HUMAN Security)
provider_slug: perimeterx
scheme_count: 1
schemes:
- applies_to:
  - Account Defender API
  - Bot Defender API
  - Credential Intelligence API
  - Code Defender API
  - PCI DSS API
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  token_types:
  - for:
    - Account Defender
    - Alerts
    - Bot Defender
    - Credential Intelligence
    name: server token
    provisioning: Created per application in HUMAN Console under Platform Settings > Applications > Application settings > Server token. Up to three server tokens per application.
  - expiry: Tokens have an expiration date; rotate before expiry.
    for:
    - Code Defender
    - PCI DSS
    name: API token
    provisioning: Retrieved from Code Defender > Settings > Integrations > Integration Settings > CD API Integration; may require HUMAN support (contact-support@humansecurity.com) to generate.
  type: http
slug: perimeterx-authentication
source_filename: perimeterx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.humansecurity.com/applications/reference/authentication\ndocs: https://docs.humansecurity.com/applications/reference/authentication\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    All Applications Protection API requests authenticate with a Bearer token in the\n    Authorization header (`authorization: Bearer <token>`). No password is used. Requests\n    without valid authentication fail. Tokens are provisioned per solution from the HUMAN Console.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  applies_to:\n  - Account Defender API\n  - Bot Defender API\n  - Credential Intelligence API\n  - Code Defender API\n  - PCI DSS API\n  token_types:\n  - name: server token\n    for: [Account Defender, Alerts, Bot Defender, Credential Intelligence]\n    provisioning: >-\n      Created per application in HUMAN\
  \ Console under Platform Settings > Applications >\n      Application settings > Server token. Up to three server tokens per application.\n  - name: API token\n    for: [Code Defender, PCI DSS]\n    provisioning: >-\n      Retrieved from Code Defender > Settings > Integrations > Integration Settings > CD API\n      Integration; may require HUMAN support (contact-support@humansecurity.com) to generate.\n    expiry: Tokens have an expiration date; rotate before expiry.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perimeterx/refs/heads/main/authentication/perimeterx-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Bot Mitigation
- Application Security
- Fraud Prevention
- Ad Fraud
- Account Takeover
- Agentic AI
- Cybersecurity
- API
---
