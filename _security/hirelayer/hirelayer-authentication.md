---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hirelayer-hirelayer-api-api-openapi.yml
  format: yaml
  label: HireLayer HireLayer API
  slug: hirelayer-hirelayer-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hirelayer/refs/heads/main/openapi/hirelayer-hirelayer-api-api-openapi.yml
- filename: hirelayer-jobs-api-openapi.yml
  format: yaml
  label: HireLayer Jobs API
  slug: hirelayer-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hirelayer/refs/heads/main/openapi/hirelayer-jobs-api-openapi.yml
- filename: hirelayer-matching-api-openapi.yml
  format: yaml
  label: HireLayer Matching API
  slug: hirelayer-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hirelayer/refs/heads/main/openapi/hirelayer-matching-api-openapi.yml
- filename: hirelayer-parser-api-openapi.yml
  format: yaml
  label: HireLayer Parser API
  slug: hirelayer-parser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hirelayer/refs/heads/main/openapi/hirelayer-parser-api-openapi.yml
- filename: hirelayer-skills-api-openapi.yml
  format: yaml
  label: HireLayer Skills API
  slug: hirelayer-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hirelayer/refs/heads/main/openapi/hirelayer-skills-api-openapi.yml
auth_types: []
description: Authenticate every request with an X-API-Key header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hirelayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: HireLayer declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: HireLayer
provider_slug: hirelayer
scheme_count: 1
schemes:
- evidence: Authenticate every request with an X-API-Key header.
  header: X-API-Key
  how_to_obtain: Create a key in Dashboard → API keys.
  location: header
  name: X-API-Key
  type: apiKey
slug: hirelayer-authentication
source_filename: hirelayer-authentication.yml
source_heading: Authentication Profile
source_url: https://hirelayer.co/api-docs/authentication.md
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hirelayer.co/api-docs/authentication.md\nsources:\n- https://hirelayer.co/api-docs/authentication.md\n- https://hirelayer.co/api-docs/quickstart.md\ndescription: Authenticate every request with an X-API-Key header.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Authenticate every request with an X-API-Key header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a key in Dashboard → API keys.\ndocs: https://hirelayer.co/api-docs/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hirelayer/refs/heads/main/authentication/hirelayer-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Recruiting
- ResumeParsing
- CandidateMatching
---
