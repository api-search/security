---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jevstation-com-openapi-generated.yml
  format: yaml
  label: JevStation API
  slug: jevstation-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jevstation-com/openapi/_ae-authored/jevstation-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: JevStation Authentication
name_suffix: Authentication
oauth_flows: []
overview: JevStation declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: JevStation
provider_slug: jevstation-com
scheme_count: 1
schemes:
- evidence: 'curl https://jevstation.com/api/v1/systemone -H "Authorization: Bearer $JEVSTATION_API_KEY" returns your credits and rate limits.'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: jevstation-com-authentication
source_filename: jevstation-com-authentication.yml
source_heading: Authentication Profile
source_url: https://jevstation.com/blog/jev-seo-audit-tool
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://jevstation.com/blog/jev-seo-audit-tool\nsources:\n- https://jevstation.com/blog/jev-seo-audit-tool\n- https://jevstation.com/blog/jev-ultrafast-browser-agent\n- https://jevstation.com/blog/cloudflare-clef-tested\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl https://jevstation.com/api/v1/systemone -H \"Authorization: Bearer $JEVSTATION_API_KEY\" returns your credits and rate limits.'\n  location: header\n  header: Authorization\ndocs: https://jevstation.com/blog/jev-seo-audit-tool\n"
source_yaml_url: https://artifacts.apis.io/jevstation-com/authentication/jevstation-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Workspace
- StructuredAnswers
- CreditMetered
---
