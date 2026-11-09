---
anonymous_access: false
api_key_in: []
api_specs:
- filename: domandata-net-openapi-generated.yml
  format: yaml
  label: Domandata API
  slug: domandata-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/domandata-net/openapi/_ae-authored/domandata-net-openapi-generated.yml
auth_types: []
description: Authentication methods as published on Domandata help pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Domandata Net Authentication
name_suffix: Authentication
oauth_flows: []
overview: Domandata declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Domandata
provider_slug: domandata-net
scheme_count: 1
schemes:
- evidence: Pass the key as a Bearer token in the Authorization header.
  header: Authorization
  how_to_obtain: Create an API key in Settings → Integrations; keys start with dmdt_
  location: header
  name: Bearer
  type: http-bearer
slug: domandata-net-authentication
source_filename: domandata-net-authentication.yml
source_heading: Authentication Profile
source_url: https://www.domandata.net/help/api-keys-survey-responses
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.domandata.net/help/api-keys-survey-responses\nsources:\n- https://www.domandata.net/help/api-keys-survey-responses\n- https://www.domandata.net/help/set-up-saved-credentials\ndescription: Authentication methods as published on Domandata help pages.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Pass the key as a Bearer token in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings → Integrations; keys start with dmdt_\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the referenced pages.\ndocs: https://www.domandata.net/help/api-keys-survey-responses\n"
source_yaml_url: https://artifacts.apis.io/domandata-net/authentication/domandata-net-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Surveys
- Academic
- Research
- Software
---
