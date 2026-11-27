---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jsmon-sh-openapi-generated.yml
  format: yaml
  label: Jsmon API
  slug: jsmon-sh-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jsmon-sh/openapi/_ae-authored/jsmon-sh-openapi-generated.yml
auth_types: []
description: Authentication schemes for Jsmon as documented.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Jsmon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jsmon declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Jsmon
provider_slug: jsmon-sh
scheme_count: 1
schemes:
- evidence: 'curl -X POST https://api.jsmon.sh/api/v1/scan \  -H "Authorization: Bearer YOUR_API_KEY" \  -H "Content-Type: application/json" \  -d ''{"type": "domain", "target": "example.com", "workspace": "WORKSPACE_ID"}'''
  header: Authorization
  how_to_obtain: Generate API key via Settings → API tab
  location: header
  name: Bearer
  type: http-bearer
slug: jsmon-sh-authentication
source_filename: jsmon-sh-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.jsmon.sh/api-keys-and-credits.md
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.jsmon.sh/api-keys-and-credits.md\nsources:\n- https://docs.jsmon.sh/api-keys-and-credits.md\ndescription: Authentication schemes for Jsmon as documented.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl -X POST https://api.jsmon.sh/api/v1/scan \\  -H \"Authorization: Bearer YOUR_API_KEY\" \\  -H \"Content-Type: application/json\" \\  -d\n    ''{\"type\": \"domain\", \"target\": \"example.com\", \"workspace\": \"WORKSPACE_ID\"}'''\n  location: header\n  header: Authorization\n  how_to_obtain: Generate API key via Settings → API tab\ndocs: https://docs.jsmon.sh/api-keys-and-credits.md\n"
source_yaml_url: https://artifacts.apis.io/jsmon-sh/authentication/jsmon-sh-authentication.yml
summary_line: 1 scheme
tags:
- Security
- Attack Surface
- Artificial Intelligence
- Monitoring
- Platform
---
