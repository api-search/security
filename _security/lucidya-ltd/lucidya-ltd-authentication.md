---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Lucidya Ltd Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lucidya Ltd declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lucidya Ltd
provider_slug: lucidya-ltd
scheme_count: 1
schemes:
- description: Programmatic access is granted through Lucidya OAuth client applications. Token/authorization endpoints and exact flow are documented per product on the product's Authorization page (linked below) and are not fully public without an account.
  header: Authorization
  in: header
  name: Lucidya OAuth client
  type: oauth2
slug: lucidya-ltd-authentication
source_filename: lucidya-ltd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.lucidya.com/\nname: Lucidya API Authentication\ntype: Authentication\nsummary: >-\n  Each Lucidya public API product carries its own authorization flow, documented\n  on a dedicated \"Authorization\" page under docs.lucidya.com. Access is\n  OAuth-based (Lucidya provisions OAuth client applications for programmatic\n  access); calls are issued against the api.lucidya.com host.\nschemes:\n- type: oauth2\n  name: Lucidya OAuth client\n  description: >-\n    Programmatic access is granted through Lucidya OAuth client applications.\n    Token/authorization endpoints and exact flow are documented per product on\n    the product's Authorization page (linked below) and are not fully public\n    without an account.\n  in: header\n  header: Authorization\ndocs:\n- product: Social Listening\n  url: https://docs.lucidya.com/docs/Social-Listening-api/uh64vtmx7x4kl-authorization\n- product: AI\n  url: https://docs.lucidya.com/docs/ai-api/sjq8uo8o8lt93-authorization\n\
  - product: CDP\n  url: https://docs.lucidya.com/docs/cdp-api/kae3rp3opgd5m-authorization\n- product: OmniChannel\n  url: https://docs.lucidya.com/docs/omnichannel-api/cfqqlsohea8mv-authorization\n- product: OmniServe Analytics\n  url: https://docs.lucidya.com/docs/omniserve/8s65uy0al6adj-authorization\nhosts:\n- https://api.lucidya.com\nnotes: >-\n  The api.lucidya.com host is live and fronted by Cloudflare Access. Exact token\n  URLs and scope names were not fully public on this pass, so they are left\n  unstated rather than guessed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucidya-ltd/refs/heads/main/authentication/lucidya-ltd-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Customer Experience
- Social Listening
- Customer Data Platform
- Analytics
- Artificial Intelligence
- Omnichannel
- Arabic NLP
- MENA
---
