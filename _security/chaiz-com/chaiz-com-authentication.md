---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chaiz-com-openapi.yml
  format: yaml
  label: Chaiz Partner API
  slug: chaiz-partner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chaiz-com/openapi/chaiz-com-openapi.yml
auth_types: []
description: Authentication uses a Bearer token sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Chaiz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chaiz declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Chaiz
provider_slug: chaiz-com
scheme_count: 1
schemes:
- evidence: 'Every Partner API request carries a Bearer token:'
  header: Authorization
  how_to_obtain: Obtain an API key via self‑service registration (POST /api/v2/Partners/Register and POST /api/v2/Partners/Register/Verify) or through managed onboarding.
  location: header
  name: Bearer
  type: http-bearer
slug: chaiz-com-authentication
source_filename: chaiz-com-authentication.yml
source_heading: Authentication Profile
source_url: https://dev-docs.chaiz.com/getting-started/authentication/index.md
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dev-docs.chaiz.com/getting-started/authentication/index.md\nsources:\n- https://dev-docs.chaiz.com/getting-started/authentication/index.md\n- https://dev-docs.chaiz.com/getting-started/authentication\n- https://dev-docs.chaiz.com/reference/api-reference/tag/api-keys/delete/api/v2/Partners/Register\n- https://dev-docs.chaiz.com/reference/api-reference/tag/api-keys/post/api/v2/Partners/Register/Rotate\ndescription: Authentication uses a Bearer token sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every Partner API request carries a Bearer token:'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain an API key via self‑service registration (POST /api/v2/Partners/Register and POST /api/v2/Partners/Register/Verify) or\n    through managed onboarding.\ndocs: https://dev-docs.chaiz.com/getting-started/authentication/index.md\n"
source_yaml_url: https://artifacts.apis.io/chaiz-com/authentication/chaiz-com-authentication.yml
summary_line: 1 scheme
tags:
- Marketplace
- Automotive
- Extended Warranty
- Digital-First
---
