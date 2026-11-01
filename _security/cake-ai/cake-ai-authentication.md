---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Cake as described in the documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cake Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cake declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cake
provider_slug: cake-ai
scheme_count: 1
schemes:
- evidence: Cake Agents uses OIDC for authentication. You can use any compliant provider, or [delegate auth to an authenticating proxy](#header-auth) via trusted headers.
  flows:
  - authorization_code
  how_to_obtain: Create a new OIDC client in your identity provider with a confidential client type, set the redirect URI to https://<controlPlane.host>/api/auth/callback/oidc, and export the client ID and secret.
  name: oidc
  scopes:
  - openid
  - email
  - profile
  type: oauth2
slug: cake-ai-authentication
source_filename: cake-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.cake.ai/admin/token-limits.md
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.cake.ai/admin/token-limits.md\nsources:\n- https://docs.cake.ai/admin/token-limits.md\n- https://docs.cake.ai/user/session-token-limits.md\n- https://docs.cake.ai/admin/getting-started-console.md\n- https://docs.cake.ai/admin/getting-started-kubernetes.md\ndescription: Authentication methods for Cake as described in the documentation.\nschemes:\n- type: oauth2\n  name: oidc\n  evidence: Cake Agents uses OIDC for authentication. You can use any compliant provider, or [delegate auth to an authenticating proxy](#header-auth)\n    via trusted headers.\n  flows:\n  - authorization_code\n  scopes:\n  - openid\n  - email\n  - profile\n  how_to_obtain: Create a new OIDC client in your identity provider with a confidential client type, set the redirect URI to https://<controlPlane.host>/api/auth/callback/oidc,\n    and export the client ID and secret.\ndocs: https://docs.cake.ai/admin/token-limits.md\n"
source_yaml_url: https://artifacts.apis.io/cake-ai/authentication/cake-ai-authentication.yml
summary_line: 1 scheme
tags:
- AI platform
- Regulated industries
- Coding agents
- Data extraction
- Enterprise AI
- Governance
- Security
---
