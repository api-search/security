---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fixragent-com-triage-api-openapi.yml
  format: yaml
  label: fixRAgent Triage API
  slug: fixragent-com-triage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixragent-com/openapi/fixragent-com-triage-api-openapi.yml
- filename: fixragent-com-usage-api-openapi.yml
  format: yaml
  label: fixRAgent Usage API
  slug: fixragent-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixragent-com/openapi/fixragent-com-usage-api-openapi.yml
auth_types: []
description: Authentication for fixRAgent uses an API key that can be sent in a header, as a Bearer token, or as a query parameter.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: fixRAgent Authentication
name_suffix: Authentication
oauth_flows: []
overview: fixRAgent declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: fixRAgent
provider_slug: fixragent-com
scheme_count: 1
schemes:
- evidence: The HTTP API, `POST https://fixragent.com/api/triage`, takes a key in the `x-triage-key` header.
  header: x-triage-key
  how_to_obtain: A key is issued to a person via the form at https://fixragent.com/docs#key; the key is emailed to the requester.
  location: header
  name: x-triage-key
  type: apiKey
slug: fixragent-com-authentication
source_filename: fixragent-com-authentication.yml
source_heading: Authentication Profile
source_url: https://fixragent.com/auth.md
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fixragent.com/auth.md\nsources:\n- https://fixragent.com/auth.md\n- https://fixragent.com/docs/AGENTS-QUICKSTART.txt\ndescription: Authentication for fixRAgent uses an API key that can be sent in a header, as a Bearer token, or as a query parameter.\nschemes:\n- type: apiKey\n  name: x-triage-key\n  evidence: The HTTP API, `POST https://fixragent.com/api/triage`, takes a key in the `x-triage-key` header.\n  location: header\n  header: x-triage-key\n  how_to_obtain: A key is issued to a person via the form at https://fixragent.com/docs#key; the key is emailed to the requester.\nnote: There is no OAuth flow; the `.well-known/oauth-*` endpoints return 404. 2 extracted row(s) were dropped because their quote was not on the\n  page.\ndocs: https://fixragent.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/fixragent-com/authentication/fixragent-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Property Management
- Photo Triage
- Maintenance
- Real Estate
---
