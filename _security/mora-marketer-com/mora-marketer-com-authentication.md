---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mora-marketer-com-discover-api-openapi.yml
  format: yaml
  label: Mora Discover API
  slug: mora-marketer-com-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mora-marketer-com/openapi/mora-marketer-com-discover-api-openapi.yml
auth_types: []
description: Mora uses OAuth 2.1 authorization-code flow with PKCE S256 for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mora Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mora declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mora
provider_slug: mora-marketer-com
scheme_count: 1
schemes:
- evidence: 'Authorization: OAuth 2.1 authorization-code flow with PKCE S256'
  flows:
  - authorization_code
  how_to_obtain: Client registration via Client ID Metadata Documents (CIMD); dynamic client registration is not exposed.
  name: OAuth 2.1
  scopes:
  - mora.read
  - mora.read.ads
  - mora.write.knowledge
  type: oauth2
slug: mora-marketer-com-authentication
source_filename: mora-marketer-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.mora-marketer.com/auth.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.mora-marketer.com/auth.md\nsources:\n- https://www.mora-marketer.com/auth.md\ndescription: Mora uses OAuth 2.1 authorization-code flow with PKCE S256 for authentication.\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: 'Authorization: OAuth 2.1 authorization-code flow with PKCE S256'\n  flows:\n  - authorization_code\n  scopes:\n  - mora.read\n  - mora.read.ads\n  - mora.write.knowledge\n  how_to_obtain: Client registration via Client ID Metadata Documents (CIMD); dynamic client registration is not exposed.\ndocs: https://www.mora-marketer.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/mora-marketer-com/authentication/mora-marketer-com-authentication.yml
summary_line: 1 scheme
tags:
- Marketing
- Software-as-a-Service
- Social Media
- Advertising
- Content Generation
- Company
---
