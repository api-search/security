---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods published on Apica documentation pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Apica Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apica declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Apica
provider_slug: apica-io
scheme_count: 1
schemes:
- evidence: 'API Keys in ascent are used to access APIs. They are embedded in the API request using the `Authorization: Bearer <api-key>` header.'
  header: Authorization
  how_to_obtain: Create an API Key via the API Key page in the UI (API Key > Create New Key) or retrieve an existing key from the API key page.
  location: header
  name: API Key
  type: apiKey
slug: apica-io-authentication
source_filename: apica-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.apica.io/admin/api-key-management.md
source_yaml: "generated: '2026-10-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.apica.io/admin/api-key-management.md\nsources:\n- https://docs.apica.io/admin/api-key-management.md\n- https://docs.apica.io/integrations/overview/generating-a-secure-ingest-token.md\n- https://docs.apica.io/platform-docs/zebratester-scripting/zebratester-user-guide/advanced-topics/credentials-manager-for-zebratester.md\n- https://docs.apica.io/platform-docs/zebratester-scripting/zebratester-how-to-articles/how-to-configure-a-zebratester-script-to-fetch-credentials-from-cyberark.md\ndescription: Authentication methods published on Apica documentation pages.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'API Keys in ascent are used to access APIs. They are embedded in the API request using the `Authorization: Bearer <api-key>` header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API Key via the API Key page in the UI (API Key >\
  \ Create New Key) or retrieve an existing key from the API key page.\nnote: No OAuth2, http‑basic, http‑bearer, JWT, HMAC, mTLS, or other authentication schemes were found in the provided pages.\ndocs: https://docs.apica.io/admin/api-key-management.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apica-io/refs/heads/main/authentication/apica-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Observability
- Telemetry
- AI
- Cloud
---
