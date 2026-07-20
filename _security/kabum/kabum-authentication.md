---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Kabum Authentication
name_suffix: Authentication
oauth_flows: []
overview: KaBum! secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KaBum!
provider_slug: kabum
scheme_count: 1
schemes:
- description: Seller API key generated in the Mirakl marketplace account under user settings -> "Chave de API" -> "Gerar uma nova chave de API". Sent as an authorization header on every request to the marketplace API. Keys can be temporarily blocked if rate limits are exceeded.
  in: header
  name: MiraklApiKey
  provisioning: https://kabum-dev.mirakl.net/login
  sources:
  - https://www.kabum.com.br/hotsite/documentacao-hubscore/
  type: apiKey
slug: kabum-authentication
source_filename: kabum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://www.kabum.com.br/hotsite/documentacao-hubscore/\ndocs: https://www.kabum.com.br/hotsite/documentacao-hubscore/\nnote: >-\n  KaBuM!'s Marketplace Seller Integration API is operated on the Mirakl platform\n  (production host marketplace-kabum.mirakl.net, development host\n  kabum-dev.mirakl.net). No OpenAPI is published by KaBuM!; this profile is\n  derived from KaBuM!'s public seller integration documentation. Authentication\n  is API-key based — each seller generates an API key in the Mirakl seller\n  account settings and sends it on every request.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: MiraklApiKey\n  type: apiKey\n  in: header\n  description: >-\n    Seller API key generated in the Mirakl marketplace account under user\n    settings -> \"Chave de API\" -> \"Gerar uma nova chave de API\". Sent as an\n    authorization header on every request to the marketplace\
  \ API. Keys can be\n    temporarily blocked if rate limits are exceeded.\n  provisioning: https://kabum-dev.mirakl.net/login\n  sources:\n  - https://www.kabum.com.br/hotsite/documentacao-hubscore/\nenvironments:\n- name: production\n  host: https://marketplace-kabum.mirakl.net\n- name: development\n  host: https://kabum-dev.mirakl.net\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kabum/refs/heads/main/authentication/kabum-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- E-Commerce
- Retail
- Marketplace
- Technology
- Electronics
- Games
- Brazil
- Seller Integration
- Mirakl
---
