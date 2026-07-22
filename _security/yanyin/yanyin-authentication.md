---
api_key_in: []
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Yanyin Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Yanyin Technology secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Yanyin Technology
provider_slug: yanyin
scheme_count: 2
schemes:
- description: API Key authentication issued and managed through the Yanyin Developer Center (密钥与凭证管理). Enforced with request signing and IP allowlisting at the API gateway.
  name: apiKey
  sources:
  - https://www.yanyin.tech/product/mega-open-platform
  type: apiKey
- description: OAuth2 Client Credentials flow for server-to-server application access, advertised on the Mega Open Platform API gateway.
  name: oauth2ClientCredentials
  scheme: clientCredentials
  sources:
  - https://www.yanyin.tech/product/mega-open-platform
  type: oauth2
slug: yanyin-authentication
source_filename: yanyin-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.yanyin.tech/product/mega-open-platform\ndocs: https://www.yanyin.tech/product/mega-open-platform#api-gateway\nsummary:\n  types: [apiKey, oauth2]\n  oauth2_flows: [clientCredentials]\n  scope_model: per-tenant and per-application authorization\nschemes:\n- name: apiKey\n  type: apiKey\n  description: >-\n    API Key authentication issued and managed through the Yanyin Developer\n    Center (密钥与凭证管理). Enforced with request signing and IP allowlisting at the\n    API gateway.\n  sources: [https://www.yanyin.tech/product/mega-open-platform]\n- name: oauth2ClientCredentials\n  type: oauth2\n  scheme: clientCredentials\n  description: >-\n    OAuth2 Client Credentials flow for server-to-server application access,\n    advertised on the Mega Open Platform API gateway.\n  sources: [https://www.yanyin.tech/product/mega-open-platform]\nnotes: >-\n  Derived from the provider's published Open Platform product page; the concrete\n\
  \  OpenAPI securitySchemes are not public (developer console is behind\n  app.yanyin.tech login).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yanyin/refs/heads/main/authentication/yanyin-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Biotechnology
- Life Sciences
- Artificial Intelligence
- Research
- Electronic Lab Notebook
- LIMS
- SaaS
- China
---
