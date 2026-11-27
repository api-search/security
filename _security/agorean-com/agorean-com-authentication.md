---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agorean-com-openapi-generated.yml
  format: yaml
  label: Agorean API
  slug: agorean-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agorean-com/openapi/_ae-authored/agorean-com-openapi-generated.yml
auth_types: []
description: Authentication schemes for Agorean API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agorean Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agorean declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Agorean
provider_slug: agorean-com
scheme_count: 1
schemes:
- evidence: 'Every other call sends your API key as a header: Authorization: Bearer agk_…'
  header: Authorization
  how_to_obtain: Create a profile (createProfile) which returns an API key prefixed with agk_
  location: header
  name: API key
  type: http-bearer
slug: agorean-com-authentication
source_filename: agorean-com-authentication.yml
source_heading: Authentication Profile
source_url: https://agorean.com/docs/keys
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agorean.com/docs/keys\nsources:\n- https://agorean.com/docs/keys\n- https://agorean.com/docs/getting-started.md\n- https://agorean.com/docs/getting-started\ndescription: Authentication schemes for Agorean API\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Every other call sends your API key as a header: Authorization: Bearer agk_…'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a profile (createProfile) which returns an API key prefixed with agk_\ndocs: https://agorean.com/docs/keys\n"
source_yaml_url: https://artifacts.apis.io/agorean-com/authentication/agorean-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Marketplace
- Reviews
- Payments
- Agents
---
