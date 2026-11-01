---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication via OAuth 2.0 token obtained from the Secrets page of a created app.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Put Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: put.io declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: put.io
provider_slug: put-io
scheme_count: 1
schemes:
- evidence: After saving, click on the **key icon** next to the app you just created. It'll take you to the **Secrets** page and here, you can copy the token created for you.
  how_to_obtain: Create an app in the API section, then on the Secrets page copy the generated token.
  name: OAuth 2.0
  type: oauth2
slug: put-io-authentication
source_filename: put-io-authentication.yml
source_heading: Authentication Profile
source_url: http://help.put.io/en/articles/4783180-two-factor-authentication-2fa.md
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: http://help.put.io/en/articles/4783180-two-factor-authentication-2fa.md\nsources:\n- http://help.put.io/en/articles/4783180-two-factor-authentication-2fa.md\n- http://help.put.io/en/articles/5972538-how-to-get-an-oauth-token-from-put-io.md\ndescription: Authentication via OAuth 2.0 token obtained from the Secrets page of a created app.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: After saving, click on the **key icon** next to the app you just created. It'll take you to the **Secrets** page and here, you can\n    copy the token created for you.\n  how_to_obtain: Create an app in the API section, then on the Secrets page copy the generated token.\ndocs: http://help.put.io/en/articles/4783180-two-factor-authentication-2fa.md\n"
source_yaml_url: https://artifacts.apis.io/put-io/authentication/put-io-authentication.yml
summary_line: 1 scheme
tags:
- Cloud Storage
- Media Streaming
- File Management
- API
- Automation
---
