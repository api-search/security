---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Proscia Authentication
name_suffix: Authentication
oauth_flows:
- saml-sso
overview: Proscia secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the saml-sso flow(s).
provider_name: Proscia
provider_slug: proscia
scheme_count: 4
schemes:
- description: Concentriq API key, generated and managed in-app by tenant administrators.
  in: header
  name: ConcentriqApiKey
  parameter_name: concentriq-api-key
  sources:
  - github.com/Proscia/proscia-ai-tools/proscia_ai_tools/concentriqlsclient.py
  type: apiKey
- bearer_format: JWT
  description: Pre-obtained JWT bearer token presented on the Authorization header.
  name: JwtBearer
  scheme: bearer
  sources:
  - github.com/Proscia/proscia-ai-tools/proscia_ai_tools/client.py
  type: http
- description: Email + password basic credentials, exchanged server-side for a JWT.
  name: BasicAuth
  scheme: basic
  sources:
  - github.com/Proscia/proscia-ai-tools/proscia_ai_tools/client.py
  type: http
- description: Enterprise single sign-on via SAML against the customer identity provider (Okta, Microsoft Authenticator/Entra). Users can authenticate directly through their IdP, bypassing the Concentriq login page.
  flow: saml-sso
  name: SamlSSO
  sources:
  - https://proscia.com/ai-ready-workflows-intelligent-annotations-more-key-updates-in-the-latest-concentriq-ls-releases/
  type: oauth2
slug: proscia-authentication
source_filename: proscia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/Proscia/proscia-ai-tools (proscia_ai_tools client) + https://proscia.com/build-on-concentriq/\ndocs: https://proscia.com/build-on-concentriq/\nsummary:\n  types: [apiKey, http, oauth2]\n  api_key_in: [header]\n  api_key_name: concentriq-api-key\n  oauth2_flows: [saml-sso]\n  notes: >-\n    The Concentriq client accepts exactly one of three auth methods: a Concentriq API key\n    (concentriq-api-key header, generated and managed in-app by admins), a pre-obtained JWT\n    bearer token, or email+password basic auth that is exchanged for a JWT. Enterprise tenants\n    federate login via SAML SSO (Okta, Microsoft/Entra) and can bypass the Concentriq login\n    page to authenticate directly through their identity provider.\nschemes:\n- name: ConcentriqApiKey\n  type: apiKey\n  in: header\n  parameter_name: concentriq-api-key\n  description: Concentriq API key, generated and managed in-app by tenant administrators.\n\
  \  sources: [github.com/Proscia/proscia-ai-tools/proscia_ai_tools/concentriqlsclient.py]\n- name: JwtBearer\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: Pre-obtained JWT bearer token presented on the Authorization header.\n  sources: [github.com/Proscia/proscia-ai-tools/proscia_ai_tools/client.py]\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Email + password basic credentials, exchanged server-side for a JWT.\n  sources: [github.com/Proscia/proscia-ai-tools/proscia_ai_tools/client.py]\n- name: SamlSSO\n  type: oauth2\n  flow: saml-sso\n  description: >-\n    Enterprise single sign-on via SAML against the customer identity provider\n    (Okta, Microsoft Authenticator/Entra). Users can authenticate directly through\n    their IdP, bypassing the Concentriq login page.\n  sources: [https://proscia.com/ai-ready-workflows-intelligent-annotations-more-key-updates-in-the-latest-concentriq-ls-releases/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proscia/refs/heads/main/authentication/proscia-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Company
- Healthcare
- Digital Pathology
- Pathology
- Life Sciences
- Precision Medicine
- Artificial Intelligence
- Medical Imaging
- Whole Slide Imaging
- Foundation Models
- Diagnostics
---
