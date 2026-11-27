---
anonymous_access: false
api_key_in: []
api_specs:
- filename: paperlink-online-v1-openapi.json
  format: json
  label: PaperLink API V1 API
  slug: paperlink-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paperlink-online/openapi/_original/paperlink-online-v1-openapi.json
auth_types: []
description: PaperLink mobile API uses HTTP Bearer authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: PaperLink Authentication
name_suffix: Authentication
oauth_flows: []
overview: PaperLink declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: PaperLink
provider_slug: paperlink-online
scheme_count: 1
schemes:
- authorize_url: https://app.paperlink.online/api/auth/mobile/authorize
  evidence: "type: http\n      scheme: bearer"
  flows:
  - authorization_code
  header: Authorization
  location: header
  name: BearerAuth
  type: http-bearer
slug: paperlink-online-authentication
source_filename: paperlink-online-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.paperlink.online/api-reference/auth/oauth-21-+-pkce-authorize-web-session.md
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.paperlink.online/api-reference/auth/oauth-21-+-pkce-authorize-web-session.md\nsources:\n- https://developers.paperlink.online/api-reference/auth/oauth-21-+-pkce-authorize-web-session.md\n- https://developers.paperlink.online/api-reference/auth/exchange-code-or-refresh-token-for-tokens.md\n- https://developers.paperlink.online/api-reference/auth/email-a-one-time-sign-in-code-native-email-flow-step-1.md\n- https://developers.paperlink.online/api-reference/auth/revoke-the-current-session-or-one-owned-session.md\ndescription: PaperLink mobile API uses HTTP Bearer authentication.\nschemes:\n- type: http-bearer\n  name: BearerAuth\n  evidence: \"type: http\\n      scheme: bearer\"\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://app.paperlink.online/api/auth/mobile/authorize\ndocs: https://developers.paperlink.online/api-reference/auth/oauth-21-+-pkce-authorize-web-session.md\n"
source_yaml_url: https://artifacts.apis.io/paperlink-online/authentication/paperlink-online-authentication.yml
summary_line: 1 scheme
tags:
- Document Analytics
- Secure Sharing
- Software-as-a-Service
- Sales Enablement
- Data Security
---
