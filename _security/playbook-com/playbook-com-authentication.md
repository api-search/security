---
anonymous_access: false
api_key_in: []
api_specs:
- filename: playbook-com-openapi-generated.yml
  format: yaml
  label: Playbook API
  slug: playbook-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/playbook-com/openapi/_ae-authored/playbook-com-openapi-generated.yml
auth_types: []
description: Playbook API uses a Bearer token sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Playbook Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Playbook declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Playbook
provider_slug: playbook-com
scheme_count: 1
schemes:
- evidence: 'Generate a token: Create an API token scoped to your workspace, then send it as a Bearer token in the Authorization header'
  header: Authorization
  how_to_obtain: Create an API token in the Playbook app via Developer → SDK
  location: header
  name: Bearer
  type: http-bearer
slug: playbook-com-authentication
source_filename: playbook-com-authentication.yml
source_heading: Authentication Profile
source_url: https://dev.playbook.com/docs/api/create-organization-board-access-token/
source_yaml: "generated: '2026-10-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dev.playbook.com/docs/api/create-organization-board-access-token/\nsources:\n- https://dev.playbook.com/docs/api/create-organization-board-access-token/\n- https://dev.playbook.com/docs/getting_started/\ndescription: Playbook API uses a Bearer token sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Generate a token: Create an API token scoped to your workspace, then send it as a Bearer token in the Authorization header'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API token in the Playbook app via Developer → SDK\ndocs: https://dev.playbook.com/docs/api/create-organization-board-access-token/\n"
source_yaml_url: https://artifacts.apis.io/playbook-com/authentication/playbook-com-authentication.yml
summary_line: 1 scheme
tags:
- Media Management
- Creative Collaboration
- Digital Asset Management
- Enterprise Software
- Marketing
---
