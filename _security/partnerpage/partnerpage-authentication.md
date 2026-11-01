---
anonymous_access: false
api_key_in: []
api_specs:
- filename: partnerpage-openapi-generated.yml
  format: yaml
  label: PartnerPage API
  slug: partnerpage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/partnerpage/openapi/_ae-authored/partnerpage-openapi-generated.yml
auth_types: []
description: All PartnerPage API authentication is done via Header Based authentication and must be used for every request to the API.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Partnerpage Authentication
name_suffix: Authentication
oauth_flows: []
overview: PartnerPage declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: PartnerPage
provider_slug: partnerpage
scheme_count: 1
schemes:
- evidence: Add parameter in the header`Authorization`
  header: Authorization
  how_to_obtain: 'Generate and access your PartnerPage API token within your account at https://directory.partnerpage.io and send it in the Authorization header as `Authorization: Token <your token>`.'
  location: header
  name: Authorization
  type: apiKey
slug: partnerpage-authentication
source_filename: partnerpage-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.partnerpage.io/authentication-1273286m0.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.partnerpage.io/authentication-1273286m0.md\nsources:\n- https://docs.partnerpage.io/authentication-1273286m0.md\n- https://support.partnerpage.io/en/articles/17607839-turn-on-api-access-and-create-api-keys\ndescription: All PartnerPage API authentication is done via Header Based authentication and must be used for every request to the API.\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: Add parameter in the header`Authorization`\n  location: header\n  header: Authorization\n  how_to_obtain: 'Generate and access your PartnerPage API token within your account at https://directory.partnerpage.io and send it in the Authorization\n    header as `Authorization: Token <your token>`.'\ndocs: https://docs.partnerpage.io/authentication-1273286m0.md\n"
source_yaml_url: https://artifacts.apis.io/partnerpage/authentication/partnerpage-authentication.yml
summary_line: 1 scheme
tags:
- Partner
- Directory
- SaaS
- B2B
- No-code
---
