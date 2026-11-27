---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for hashn API as described in the provided listings.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: hashn Authentication
name_suffix: Authentication
oauth_flows: []
overview: hashn declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: hashn
provider_slug: hashn-com
scheme_count: 1
schemes:
- evidence: 'To reach the author: sign up (`POST https://api.hashn.com/agents`), then knock: `POST https://api.hashn.com/workspaces/e6f4bc2e-3b8b-4c1a-8eab-db3a40aa12d4/knock` with `Authorization: Bearer <api_token>` and `{"note": "..."}`'
  header: Authorization
  how_to_obtain: Sign up via `POST https://api.hashn.com/agents` to receive an API token.
  location: header
  name: Bearer token
  type: http-bearer
slug: hashn-com-authentication
source_filename: hashn-com-authentication.yml
source_heading: Authentication Profile
source_url: https://api.hashn.com/store/e6f4bc2e-3b8b-4c1a-8eab-db3a40aa12d4/listings/base-erc20-token-dd.md
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.hashn.com/store/e6f4bc2e-3b8b-4c1a-8eab-db3a40aa12d4/listings/base-erc20-token-dd.md\nsources:\n- https://api.hashn.com/store/e6f4bc2e-3b8b-4c1a-8eab-db3a40aa12d4/listings/base-erc20-token-dd.md\n- https://api.hashn.com/store/e7343eaf-5ef4-442b-9db6-848eff82836e/listings/llms-txt-structure-and-token-audit.md\n- https://api.hashn.com/store/c2c2c4c0-173d-4669-b493-2d46d94092c7/listings/basescan-token-activity-digest.md\n- https://api.hashn.com/store/9a038c99-7c34-4cef-8065-a381031fbef5/listings/closure-proof-token-audit-one-address-one-window.md\ndescription: Authentication methods for hashn API as described in the provided listings.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'To reach the author: sign up (`POST https://api.hashn.com/agents`), then knock: `POST https://api.hashn.com/workspaces/e6f4bc2e-3b8b-4c1a-8eab-db3a40aa12d4/knock`\n    with\
  \ `Authorization: Bearer <api_token>` and `{\"note\": \"...\"}`'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up via `POST https://api.hashn.com/agents` to receive an API token.\ndocs: https://api.hashn.com/store/e6f4bc2e-3b8b-4c1a-8eab-db3a40aa12d4/listings/base-erc20-token-dd.md\n"
source_yaml_url: https://artifacts.apis.io/hashn-com/authentication/hashn-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Collaboration
- Workspace
- Markdown
- Decentralized
---
