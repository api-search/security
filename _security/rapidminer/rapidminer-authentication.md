---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Rapidminer Authentication
name_suffix: Authentication
oauth_flows:
- refresh_token
overview: Rapidminer secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the refresh_token flow(s).
provider_name: Rapidminer
provider_slug: rapidminer
scheme_count: 2
schemes:
- description: Long-lived offline (refresh) token issued by the AI Hub authentication server, exchanged with a client_secret for access tokens. Configured on the Server/Connections/Scoring classes via authentication_server, offline_token, and client_secret parameters.
  flow: refresh_token
  name: aiHubOfflineToken
  parameters:
    authentication_server: URL of the AI Hub auth server (e.g. https://host:8081/auth)
    client_secret: client secret paired with the offline token
    offline_token: long-lived offline/refresh token
  sources:
  - README.md
  type: oauth2
- description: AI Hub Vault stores sensitive connection field values; encrypted connection values are injected transparently when a Server instance is provided.
  name: aiHubVault
  sources:
  - README.md
  type: other
slug: rapidminer-authentication
source_filename: rapidminer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/rapidminer/python-rapidminer/blob/master/README.md\nnotes: >-\n  No public OpenAPI/securitySchemes were found; this profile is derived from the\n  official python-rapidminer client documentation. Altair AI Hub authenticates\n  clients via OAuth against a Keycloak-style authentication server. From package\n  version 10.2.0, username/password OAuth for the WebApi and Server classes was\n  removed in favor of the offline token (refresh token) method. SAML\n  authentication on AI Hub is not supported by the Python client.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [refresh_token]\nschemes:\n- name: aiHubOfflineToken\n  type: oauth2\n  flow: refresh_token\n  description: >-\n    Long-lived offline (refresh) token issued by the AI Hub authentication\n    server, exchanged with a client_secret for access tokens. Configured on the\n    Server/Connections/Scoring classes via authentication_server, offline_token,\n\
  \    and client_secret parameters.\n  parameters:\n    authentication_server: URL of the AI Hub auth server (e.g. https://host:8081/auth)\n    offline_token: long-lived offline/refresh token\n    client_secret: client secret paired with the offline token\n  sources: [README.md]\n- name: aiHubVault\n  type: other\n  description: >-\n    AI Hub Vault stores sensitive connection field values; encrypted connection\n    values are injected transparently when a Server instance is provided.\n  sources: [README.md]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidminer/refs/heads/main/authentication/rapidminer-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Ai
- Machine Learning
- Data Science
- Predictive Analytics
- Data Preparation
- Model Deployment
- Analytics
---
