---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lovisa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lovisa declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lovisa
provider_slug: lovisa
scheme_count: 2
schemes:
- evidence: '"Server-to-server requests and hosted or remote browsers must use [Web Bot Auth](https://shopify.dev/docs/api/storefront#identifying-bots-with-web-bot-auth) and follow the service''s authentication requirements."'
  name: Web Bot Auth (agent identification)
  source: https://www.lovisa.com/llms.txt
  type: http-message-signatures
- evidence: 'UCP profile capability dev.ucp.common.identity_linking; llms.txt: "Connect their Shop account for personalized discovery and accelerated checkout with saved details."'
  name: UCP identity linking (buyer Shop account)
  note: Flow details are defined by the UCP spec and Shopify, not documented by Lovisa; type is the UCP identity-linking mechanism as published by ucp.dev, not observed.
  source: https://www.lovisa.com/.well-known/ucp
  type: oauth2
slug: lovisa-authentication
source_filename: lovisa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: searched\nsource: https://www.lovisa.com/llms.txt\ndocs: https://shopify.dev/docs/api/storefront#identifying-bots-with-web-bot-auth\nsummary: Lovisa publishes no API auth reference of its own. Its llms.txt (Shopify-generated) says agent traffic\n  to the UCP MCP service must identify itself, server-to-server requests using Web Bot Auth, and that buyers may\n  connect a Shop account. The store's UCP profile advertises the dev.ucp.common.identity_linking capability. The\n  anonymous tools/list recorded in json-schema/ on 2026-10-21 answered without credentials.\nschemes:\n- name: Web Bot Auth (agent identification)\n  type: http-message-signatures\n  evidence: '\"Server-to-server requests and hosted or remote browsers must use [Web Bot Auth](https://shopify.dev/docs/api/storefront#identifying-bots-with-web-bot-auth)\n    and follow the service''s authentication requirements.\"'\n  source: https://www.lovisa.com/llms.txt\n- name: UCP identity linking\
  \ (buyer Shop account)\n  type: oauth2\n  evidence: 'UCP profile capability dev.ucp.common.identity_linking; llms.txt: \"Connect their Shop account for\n    personalized discovery and accelerated checkout with saved details.\"'\n  source: https://www.lovisa.com/.well-known/ucp\n  note: Flow details are defined by the UCP spec and Shopify, not documented by Lovisa; type is the UCP identity-linking\n    mechanism as published by ucp.dev, not observed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lovisa/refs/heads/main/authentication/lovisa-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Retail
- Jewelry
- Fashion
- E-Commerce
- Australia
- ASX Listed
---
