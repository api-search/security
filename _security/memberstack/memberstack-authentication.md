---
anonymous_access: false
api_key_in: []
api_specs:
- filename: memberstack-openapi-generated.yml
  format: yaml
  label: Memberstack API
  slug: memberstack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memberstack/openapi/_ae-authored/memberstack-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Memberstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Memberstack declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Memberstack
provider_slug: memberstack
scheme_count: 2
schemes:
- description: Public key used in the DOM package for client-side authentication (starts with pk_ or pk_sb_).
  in: code
  name: publicKey
  type: apiKey
- description: Secret key used in the Admin packages for server-side authentication (starts with sk_ or sk_sb_).
  in: code
  name: secretKey
  type: apiKey
slug: memberstack-authentication
source_filename: memberstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://developers.memberstack.com/admin-rest-api/quick-start.md\nschemes:\n  - type: apiKey\n    name: \"publicKey\"\n    in: \"code\"\n    description: \"Public key used in the DOM package for client-side authentication (starts with pk_ or pk_sb_).\"\n  - type: apiKey\n    name: \"secretKey\"\n    in: \"code\"\n    description: \"Secret key used in the Admin packages for server-side authentication (starts with sk_ or sk_sb_).\"\n"
source_yaml_url: https://artifacts.apis.io/memberstack/authentication/memberstack-authentication.yml
summary_line: 2 schemes
tags:
- Membership
- Webflow
- SaaS
- Authentication
- Payments
---
