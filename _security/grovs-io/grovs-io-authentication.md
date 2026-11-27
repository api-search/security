---
anonymous_access: false
api_key_in: []
api_specs:
- filename: grovs-io-openapi-generated.yml
  format: yaml
  label: grovs API
  slug: grovs-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grovs-io/openapi/_ae-authored/grovs-io-openapi-generated.yml
auth_types: []
description: Authentication methods for Grovs API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: grovs Authentication
name_suffix: Authentication
oauth_flows: []
overview: grovs declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: grovs
provider_slug: grovs-io
scheme_count: 2
schemes:
- evidence: PROJECT-KEY and ENVIRONMENT headers
  header: PROJECT-KEY
  how_to_obtain: 'Find it in the dashboard under Developers › API Key. One key covers both environments; the ENVIRONMENT header picks the project: production or test.'
  location: header
  name: Project key
  type: apiKey
- evidence: 'Authorization: Bearer <key>'
  header: Authorization
  how_to_obtain: An instance admin creates it in the dashboard (Developers › Data Export › Pull feed tokens › Create feed token for feed tokens, or Settings › Audit Logs › Export tokens › Create token for export tokens).
  location: header
  name: Scoped key
  type: http-bearer
slug: grovs-io-authentication
source_filename: grovs-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.grovs.io/docs/api-reference/authentication.md
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.grovs.io/docs/api-reference/authentication.md\nsources:\n- https://docs.grovs.io/docs/api-reference/authentication.md\n- https://docs.grovs.io/docs/api-reference/authentication\n- https://docs.grovs.io/docs/getting-started.md\n- https://docs.grovs.io/docs/getting-started/introduction.md\ndescription: Authentication methods for Grovs API\nschemes:\n- type: apiKey\n  name: Project key\n  evidence: PROJECT-KEY and ENVIRONMENT headers\n  location: header\n  header: PROJECT-KEY\n  how_to_obtain: 'Find it in the dashboard under Developers › API Key. One key covers both environments; the ENVIRONMENT header picks the project:\n    production or test.'\n- type: http-bearer\n  name: Scoped key\n  evidence: 'Authorization: Bearer <key>'\n  location: header\n  header: Authorization\n  how_to_obtain: An instance admin creates it in the dashboard (Developers › Data Export › Pull\
  \ feed tokens › Create feed token for feed tokens,\n    or Settings › Audit Logs › Export tokens › Create token for export tokens).\ndocs: https://docs.grovs.io/docs/api-reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/grovs-io/authentication/grovs-io-authentication.yml
summary_line: 2 schemes
tags:
- Self-Hosted
- Deep Linking
- Analytics
- Mobile
- Messaging
---
