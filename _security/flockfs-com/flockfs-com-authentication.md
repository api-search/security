---
anonymous_access: false
api_key_in: []
api_specs:
- filename: flockfs-com-openapi-generated.yml
  format: yaml
  label: flockfs API
  slug: flockfs-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flockfs-com/openapi/_ae-authored/flockfs-com-openapi-generated.yml
auth_types: []
description: Authentication is performed using a bearer token sent in the Authorization header. The token can be obtained via the flockfs login sign‑in flow or from a token file/environment variable.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: flockfs Authentication
name_suffix: Authentication
oauth_flows: []
overview: flockfs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: flockfs
provider_slug: flockfs-com
scheme_count: 1
schemes:
- evidence: 'Remote/cloud agents: POST https://app.flockfs.com/mcp with Authorization: Bearer <token>'
  header: Authorization
  how_to_obtain: Obtain the token by running `flockfs login` in a browser (sign‑in link) or by creating an agent token in the web app (POST /api/tokens) and storing it in FLOCKFS_TOKEN or FLOCKFS_TOKEN_FILE.
  location: header
  name: Bearer token
  type: http-bearer
slug: flockfs-com-authentication
source_filename: flockfs-com-authentication.yml
source_heading: Authentication Profile
source_url: https://flockfs.com/docs/agent-setup/
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://flockfs.com/docs/agent-setup/\nsources:\n- https://flockfs.com/docs/agent-setup/\ndescription: Authentication is performed using a bearer token sent in the Authorization header. The token can be obtained via the flockfs login\n  sign‑in flow or from a token file/environment variable.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Remote/cloud agents: POST https://app.flockfs.com/mcp with Authorization: Bearer <token>'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain the token by running `flockfs login` in a browser (sign‑in link) or by creating an agent token in the web app (POST /api/tokens)\n    and storing it in FLOCKFS_TOKEN or FLOCKFS_TOKEN_FILE.\ndocs: https://flockfs.com/docs/agent-setup/\n"
source_yaml_url: https://artifacts.apis.io/flockfs-com/authentication/flockfs-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Real-Time
- Filesystem
- Collaboration
- Artificial Intelligence
---
