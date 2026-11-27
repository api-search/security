---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lucernanoetica-com-openapi-generated.yml
  format: yaml
  label: Lucerna Noetica API
  slug: lucernanoetica-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lucernanoetica-com/openapi/_ae-authored/lucernanoetica-com-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lucerna Noetica Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lucerna Noetica declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lucerna Noetica
provider_slug: lucernanoetica-com
scheme_count: 2
schemes:
- evidence: Operating a shop needs OAuth 2.1 with PKCE (S256), or a shop key issued from the owner's dashboard.
  flows:
  - authorization_code
  name: OAuth 2.1 with PKCE
  type: oauth2
- evidence: Operating a shop needs OAuth 2.1 with PKCE (S256), or a shop key issued from the owner's dashboard.
  how_to_obtain: Issued from the owner's dashboard
  name: Shop key
  type: http-bearer
slug: lucernanoetica-com-authentication
source_filename: lucernanoetica-com-authentication.yml
source_heading: Authentication Profile
source_url: https://lucernanoetica.com/docs
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lucernanoetica.com/docs\nsources:\n- https://lucernanoetica.com/docs\ndescription: Authentication\nschemes:\n- type: oauth2\n  name: OAuth 2.1 with PKCE\n  evidence: Operating a shop needs OAuth 2.1 with PKCE (S256), or a shop key issued from the owner's dashboard.\n  flows:\n  - authorization_code\n- type: http-bearer\n  name: Shop key\n  evidence: Operating a shop needs OAuth 2.1 with PKCE (S256), or a shop key issued from the owner's dashboard.\n  how_to_obtain: Issued from the owner's dashboard\ndocs: https://lucernanoetica.com/docs\n"
source_yaml_url: https://artifacts.apis.io/lucernanoetica-com/authentication/lucernanoetica-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- E-Commerce
- Artificial Intelligence
- online-shop
- Platform
---
