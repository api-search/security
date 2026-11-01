---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Prelude as described in the support documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Preludesecurity Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prelude declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Prelude
provider_slug: preludesecurity-com
scheme_count: 1
schemes:
- authorize_url: https://api.<region>.preludesecurity.com/iam/account/login
  evidence: As part of this change to Prelude’s authentication, accounts using custom OIDC will need to update their OAuth 2.0 Client IDs’ “Authorized Redirect URIs”.
  how_to_obtain: Configure OIDC client with Client Id, Client Secret, and redirect_uri as documented; obtain credentials from Identity Provider.
  name: Custom OIDC
  type: oauth2
slug: preludesecurity-com-authentication
source_filename: preludesecurity-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.originhq.com/research/windows-arm64-internals-deconstructing-pointer-authentication
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.originhq.com/research/windows-arm64-internals-deconstructing-pointer-authentication\nsources:\n- https://www.originhq.com/research/windows-arm64-internals-deconstructing-pointer-authentication\n- https://www.originhq.com/investigations/the-api-key-hunter\n- https://support.preludesecurity.com/docs/authentication-changes-and-requirements\n- https://support.preludesecurity.com/docs/where-do-i-find-my-openid-credentials\ndescription: Authentication methods for Prelude as described in the support documentation.\nschemes:\n- type: oauth2\n  name: Custom OIDC\n  evidence: As part of this change to Prelude’s authentication, accounts using custom OIDC will need to update their OAuth 2.0 Client IDs’ “Authorized\n    Redirect URIs”.\n  authorize_url: https://api.<region>.preludesecurity.com/iam/account/login\n  how_to_obtain: Configure OIDC client with Client Id, Client Secret,\
  \ and redirect_uri as documented; obtain credentials from Identity Provider.\ndocs: https://www.originhq.com/research/windows-arm64-internals-deconstructing-pointer-authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/preludesecurity-com/authentication/preludesecurity-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Observability
- Monitoring
- Platform
---
