---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Zoho APIs as described in the provided pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Deluge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deluge declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Deluge
provider_slug: deluge
scheme_count: 1
schemes:
- evidence: Zoho's OAuth implementation uses Bearer authentication scheme , hence while making API calls, the access token has to be passed in the Authorization header with the prefix Bearer .
  flows:
  - authorization_code
  - client_credentials
  header: Authorization
  how_to_obtain: Create a self client in API console to get a Client ID and Client Secret.
  location: header
  name: Bearer
  type: http-bearer
slug: deluge-authentication
source_filename: deluge-authentication.yml
source_heading: Authentication Profile
source_url: https://www.zoho.com/developer/oauth/self-client/overview.html
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.zoho.com/developer/oauth/self-client/overview.html\nsources:\n- https://www.zoho.com/developer/oauth/self-client/overview.html\n- https://www.zoho.com/developer/oauth/introduction.html\n- https://www.zoho.com/developer/oauth/multi-dc-support.html\n- https://www.zoho.com/developer/oauth/incremental-authorization/overview.html\ndescription: Authentication methods for Zoho APIs as described in the provided pages.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Zoho's OAuth implementation uses Bearer authentication scheme , hence while making API calls, the access token has to be passed in\n    the Authorization header with the prefix Bearer .\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  - client_credentials\n  how_to_obtain: Create a self client in API console to get a Client ID and Client Secret.\ndocs: https://www.zoho.com/developer/oauth/self-client/overview.html\n"
source_yaml_url: https://artifacts.apis.io/deluge/authentication/deluge-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Low-code
- Scripting
- Automation
- Zoho
- Serverless
---
