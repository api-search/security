---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication is performed by sending an API key in the Authorization header using the Bearer scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Emailchaser Authentication
name_suffix: Authentication
oauth_flows: []
overview: Emailchaser declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Emailchaser
provider_slug: emailchaser-com
scheme_count: 1
schemes:
- evidence: 'Every request carries your API key in the Authorization header, with the word Bearer and a space in front of it:'
  header: Authorization
  how_to_obtain: Create a key on the API & MCP page; the key looks like run_ followed by 8 letters or digits, an underscore and 40 more letters or digits.
  location: header
  name: Bearer
  type: apiKey
slug: emailchaser-com-authentication
source_filename: emailchaser-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.emailchaser.com/docs/getting-started/authentication
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.emailchaser.com/docs/getting-started/authentication\nsources:\n- https://www.emailchaser.com/docs/getting-started/authentication\n- https://www.emailchaser.com/docs/api-reference/setup\n- https://www.emailchaser.com/docs/api-reference/workspace\n- https://www.emailchaser.com/docs/getting-started/start-here\ndescription: Authentication is performed by sending an API key in the Authorization header using the Bearer scheme.\nschemes:\n- type: apiKey\n  name: Bearer\n  evidence: 'Every request carries your API key in the Authorization header, with the word Bearer and a space in front of it:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key on the API & MCP page; the key looks like run_ followed by 8 letters or digits, an underscore and 40 more letters\n    or digits.\nnote: No OAuth2, http-bearer, http-basic, jwt, hmac, mtls, or other schemes are\
  \ documented.\ndocs: https://www.emailchaser.com/docs/getting-started/authentication\n"
source_yaml_url: https://artifacts.apis.io/emailchaser-com/authentication/emailchaser-com-authentication.yml
summary_line: 1 scheme
tags:
- Cold Email
- Sales
- Marketing
- Lead Generation
- Software-as-a-Service
---
