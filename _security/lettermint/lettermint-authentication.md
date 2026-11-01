---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication for Lettermint APIs uses a Bearer token sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Lettermint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lettermint declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lettermint
provider_slug: lettermint
scheme_count: 1
schemes:
- evidence: '`--header ''Authorization: Bearer <token>''`'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: lettermint-authentication
source_filename: lettermint-authentication.yml
source_heading: Authentication Profile
source_url: https://lettermint.co/roadmap/ip-restrictions-tokens.md
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lettermint.co/roadmap/ip-restrictions-tokens.md\nsources:\n- https://lettermint.co/roadmap/ip-restrictions-tokens.md\n- https://lettermint.co/changelog/restrict-your-api-tokens-to-specific-ip-addresses.md\n- https://lettermint.co/docs/api-reference/team/project\n- https://lettermint.co/docs/api-reference/team/webhook\ndescription: Authentication for Lettermint APIs uses a Bearer token sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '`--header ''Authorization: Bearer <token>''`'\n  location: header\n  header: Authorization\ndocs: https://lettermint.co/roadmap/ip-restrictions-tokens.md\n"
source_yaml_url: https://artifacts.apis.io/lettermint/authentication/lettermint-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Email
- Transactional
- API
- European
---
