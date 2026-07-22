---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Mandiant Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Mandiant secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Mandiant
provider_slug: mandiant
scheme_count: 2
schemes:
- description: API key ID and secret issued in the Mandiant Advantage console. Used to obtain a bearer access token via the token endpoint.
  in: header
  name: mandiant_api_key
  sources:
  - https://docs.mandiant.com/home/mati-threat-intelligence-api-v3
  type: apiKey
- description: 'Access token returned from the token exchange, presented on the Authorization: Bearer header. Tokens are short-lived and must be refreshed.'
  flow: clientCredentials
  name: bearer_token
  sources:
  - https://docs.mandiant.com/home/mati-threat-intelligence-api-v3
  type: oauth2
slug: mandiant-authentication
source_filename: mandiant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.mandiant.com/home/mati-threat-intelligence-api-v3\ndocs: https://docs.mandiant.com\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    Mandiant Advantage APIs use an API key (public key) and secret pair issued in\n    the Mandiant Advantage console. The key and secret are exchanged for a\n    short-lived bearer access token via a token endpoint using an OAuth2\n    client-credentials style grant; the returned access_token is then sent on the\n    Authorization: Bearer header for subsequent API requests. The Security\n    Validation (MSV) API issues its own API key (\"Creating a Security Validation\n    API Key\" in the docs). Derivation was not possible mechanically because\n    Mandiant publishes no public OpenAPI specification; this profile is captured\n    from the public documentation.\nschemes:\n- name: mandiant_api_key\n  type: apiKey\n\
  \  in: header\n  description: >-\n    API key ID and secret issued in the Mandiant Advantage console. Used to\n    obtain a bearer access token via the token endpoint.\n  sources:\n  - https://docs.mandiant.com/home/mati-threat-intelligence-api-v3\n- name: bearer_token\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    Access token returned from the token exchange, presented on the\n    Authorization: Bearer header. Tokens are short-lived and must be refreshed.\n  sources:\n  - https://docs.mandiant.com/home/mati-threat-intelligence-api-v3\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mandiant/refs/heads/main/authentication/mandiant-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Security
- Threat Intelligence
- Cybersecurity
- Incident Response
- Attack Surface Management
- Vulnerability Intelligence
- Malware
- Google Cloud
---
