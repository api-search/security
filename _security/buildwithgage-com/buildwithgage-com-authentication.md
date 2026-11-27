---
anonymous_access: false
api_key_in: []
api_specs:
- filename: buildwithgage-com-openapi-generated.yml
  format: yaml
  label: Gage API
  slug: buildwithgage-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildwithgage-com/openapi/_ae-authored/buildwithgage-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Gage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gage declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Gage
provider_slug: buildwithgage-com
scheme_count: 1
schemes:
- evidence: 'curl -X POST https://buildwithgage.com/api/v1/quotes \ -H "Authorization: Bearer $GAGE_API_KEY" \'
  header: Authorization
  how_to_obtain: Create a test key in the dashboard after signing in; keys are provided via email invitation or generated in the developer dashboard.
  location: header
  name: Bearer
  type: http-bearer
slug: buildwithgage-com-authentication
source_filename: buildwithgage-com-authentication.yml
source_heading: Authentication Profile
source_url: https://buildwithgage.com/docs/partners/getting-started
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://buildwithgage.com/docs/partners/getting-started\nsources:\n- https://buildwithgage.com/docs/partners/getting-started\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl -X POST https://buildwithgage.com/api/v1/quotes \\ -H \"Authorization: Bearer $GAGE_API_KEY\" \\'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a test key in the dashboard after signing in; keys are provided via email invitation or generated in the developer dashboard.\ndocs: https://buildwithgage.com/docs/partners/getting-started\n"
source_yaml_url: https://artifacts.apis.io/buildwithgage-com/authentication/buildwithgage-com-authentication.yml
summary_line: 1 scheme
tags:
- Construction
- Marketplace
- Steel
- Developers
---
