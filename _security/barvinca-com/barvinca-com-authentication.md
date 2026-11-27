---
anonymous_access: false
api_key_in: []
api_specs:
- filename: barvinca-com-openapi-generated.yml
  format: yaml
  label: Barvinca API
  slug: barvinca-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/barvinca-com/openapi/_ae-authored/barvinca-com-openapi-generated.yml
auth_types: []
description: Authentication schemes for Barvinca as described on the documentation pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Barvinca Authentication
name_suffix: Authentication
oauth_flows: []
overview: Barvinca declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Barvinca
provider_slug: barvinca-com
scheme_count: 2
schemes:
- evidence: Sign in with Autodesk OAuth; Barvinca has no separate password. Sign-in uses the Autodesk authorization-code flow with PKCE (3-legged authorization).
  flows:
  - authorization_code
  how_to_obtain: User signs in with their Autodesk account using the authorization‑code flow with PKCE.
  name: Autodesk 3-Legged OAuth
  type: oauth2
- evidence: Barvinca's managed APS application uses separate server-side client-credentials authorization (2-legged).
  flows:
  - client_credentials
  how_to_obtain: Barvinca uses its server‑side client secret; the client secret is not provided to customers.
  name: Autodesk 2-Legged OAuth
  type: oauth2
slug: barvinca-com-authentication
source_filename: barvinca-com-authentication.yml
source_heading: Authentication Profile
source_url: https://barvinca.com/help/authentication
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://barvinca.com/help/authentication\nsources:\n- https://barvinca.com/help/authentication\n- https://barvinca.com/news/bulk-user-manager-token-positioning\n- https://barvinca.com/setup.md\ndescription: Authentication schemes for Barvinca as described on the documentation pages.\nschemes:\n- type: oauth2\n  name: Autodesk 3-Legged OAuth\n  evidence: Sign in with Autodesk OAuth; Barvinca has no separate password. Sign-in uses the Autodesk authorization-code flow with PKCE (3-legged\n    authorization).\n  flows:\n  - authorization_code\n  how_to_obtain: User signs in with their Autodesk account using the authorization‑code flow with PKCE.\n- type: oauth2\n  name: Autodesk 2-Legged OAuth\n  evidence: Barvinca's managed APS application uses separate server-side client-credentials authorization (2-legged).\n  flows:\n  - client_credentials\n  how_to_obtain: Barvinca uses its server‑side\
  \ client secret; the client secret is not provided to customers.\ndocs: https://barvinca.com/help/authentication\n"
source_yaml_url: https://artifacts.apis.io/barvinca-com/authentication/barvinca-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- BulkUserManagement
- Autodesk
- BIM360
- Automation
---
