---
api_key_in:
- header
api_specs:
- filename: partstech-api-openapi.yml
  format: yaml
  label: PartsTech External API
  slug: partstech-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/partstech/refs/heads/main/openapi/partstech-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Partstech Authentication
name_suffix: Authentication
oauth_flows: []
overview: PartsTech secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PartsTech
provider_slug: partstech
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: "Get access to data while protecting your account credentials.\nToken (a JWT token) are also a safer and more secure way to give you access.\n\nIt provides two ways of access:\n - `user` - Give an access to user methods.\n - `partner` - Give an acess to partner methods.\n\nTo use this way you need:\n1. Get an access token. See [\"Authentication and Access\"](#operation/getAcessToken).\n2. Add a header in the "
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/partstech-api-openapi.yml
  type: http
- description: "It is a deprecated way to get access to the methods, used only in the methods, that were in the previous version.\n\nIt provides two ways of an access:\n - `user` - Give access to user methods.\n - `partner` - Give acess to partner methods.\n\nTo use this way you need to add credentials in the request body, where it is allowed, in a next format:\n - for user methods:\n```\n\"credentials\": {\n    \"user\": {\n  "
  in: header
  name: apiKeyAuth
  parameter: credentials
  sources:
  - openapi/partstech-api-openapi.yml
  type: apiKey
slug: partstech-authentication
source_filename: partstech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/partstech-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: \"Get access to data while protecting your account credentials.\\nToken (a JWT\\\n    \\ token) are also a safer and more secure way to give you access.\\n\\nIt provides two ways\\\n    \\ of access:\\n - `user` - Give an access to user methods.\\n - `partner` - Give an acess\\\n    \\ to partner methods.\\n\\nTo use this way you need:\\n1. Get an access token. See [\\\"Authentication\\\n    \\ and Access\\\"](#operation/getAcessToken).\\n2. Add a header in the \"\n  sources:\n  - openapi/partstech-api-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: credentials\n  description: \"It is a deprecated way to get access to the methods, used only in the methods,\\\n    \\ that were in the previous version.\\\
  n\\nIt provides two ways of an access:\\n - `user` -\\\n    \\ Give access to user methods.\\n - `partner` - Give acess to partner methods.\\n\\nTo use\\\n    \\ this way you need to add credentials in the request body, where it is allowed, in a next\\\n    \\ format:\\n - for user methods:\\n```\\n\\\"credentials\\\": {\\n    \\\"user\\\": {\\n  \"\n  sources:\n  - openapi/partstech-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/partstech/refs/heads/main/authentication/partstech-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Automotive
- Auto Parts
- Parts Procurement
- Tires
- E-Commerce
- Ordering
- Catalog
- Vehicle Data
- VIN Decoding
- Shop Management
- Punchout
- Marketplace
- Supply Chain
---
