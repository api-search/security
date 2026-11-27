---
anonymous_access: false
api_key_in: []
api_specs:
- filename: slb-openapi-generated.yml
  format: yaml
  label: SLB API
  slug: slb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/slb/openapi/_ae-authored/slb-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: SLB Authentication
name_suffix: Authentication
oauth_flows: []
overview: SLB declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SLB
provider_slug: slb
scheme_count: 1
schemes:
- evidence: The Authorization HTTP header set by the UI to access the backend should be Bearer XXX
  header: Authorization
  location: header
  name: JWT
  type: http-bearer
slug: slb-authentication
source_filename: slb-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.slb.com/apis/api-tryit-usingoauthplayground.md
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.slb.com/apis/api-tryit-usingoauthplayground.md\nsources:\n- https://developer.slb.com/apis/api-tryit-usingoauthplayground.md\n- https://developer.slb.com/guides/cloud-apis/developer-portal/oauth-playground.md\n- https://developer.slb.com/solutions/ivaap/tutorials/ivaap-api-for-authentication.md\n- https://developer.slb.com/solutions/ivaap/tutorials/oauth2-authentication.md\nschemes:\n- type: http-bearer\n  name: JWT\n  evidence: The Authorization HTTP header set by the UI to access the backend should be Bearer XXX\n  location: header\n  header: Authorization\ndocs: https://developer.slb.com/apis/api-tryit-usingoauthplayground.md\n"
source_yaml_url: https://artifacts.apis.io/slb/authentication/slb-authentication.yml
summary_line: 1 scheme
tags:
- Energy
- Oilfield Services
- Engineering
---
