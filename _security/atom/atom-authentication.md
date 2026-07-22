---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Atom Authentication
name_suffix: Authentication
oauth_flows: []
overview: ATOM secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ATOM
provider_slug: atom
scheme_count: 1
schemes:
- description: Account API key issued from the Atom admin panel, sent on each request to the Atom Customers and WhatsApp template-message APIs.
  in: header
  name: apiKey
  sources:
  - https://soporte.atomchat.io/knowledge/api-de-clientes
  type: apiKey
slug: atom-authentication
source_filename: atom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://soporte.atomchat.io/knowledge/api-de-clientes\ndocs: https://soporte.atomchat.io/knowledge/api-de-clientes\nnotes: >-\n  No OpenAPI is published for the Atom (atomchat.io) API, so this profile is\n  captured from the provider's knowledge base rather than derived from a spec.\n  The Atom Customers API and WhatsApp template-message API are called over HTTPS\n  and authenticated with an account API key generated in the Atom admin panel and\n  supplied on each HTTP request (documented via the knowledge-base articles on\n  configuring the key in Postman / HTTP requests). Header name and exact placement\n  are not published in the public docs and are intentionally left unspecified here\n  rather than guessed.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  description: >-\n    Account API key issued from the Atom admin panel, sent on\
  \ each request to the\n    Atom Customers and WhatsApp template-message APIs.\n  sources:\n  - https://soporte.atomchat.io/knowledge/api-de-clientes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atom/refs/heads/main/authentication/atom-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Messaging
- WhatsApp
- Artificial Intelligence
- Conversational Commerce
- Chatbots
- Sales
- Lead Generation
- Customer Engagement
- Latin America
---
