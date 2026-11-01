---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Couchdrop API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Couchdrop Authentication
name_suffix: Authentication
oauth_flows: []
overview: Couchdrop declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Couchdrop
provider_slug: couchdrop
scheme_count: 1
schemes:
- evidence: Authenticating with Couchdrops API requires a username and password and on success returns a new authentication token.
  how_to_obtain: POST https://api.couchdrop.io/authenticate with username and password in the request body
  name: Bearer Token
  type: http-bearer
slug: couchdrop-authentication
source_filename: couchdrop-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.couchdrop.io/domains-and-accounts/authentication.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.couchdrop.io/domains-and-accounts/authentication.md\nsources:\n- https://developers.couchdrop.io/domains-and-accounts/authentication.md\n- https://docs.couchdrop.io/administration/api-tokens\ndescription: Authentication schemes for Couchdrop API\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: Authenticating with Couchdrops API requires a username and password and on success returns a new authentication token.\n  how_to_obtain: POST https://api.couchdrop.io/authenticate with username and password in the request body\ndocs: https://developers.couchdrop.io/domains-and-accounts/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/couchdrop/authentication/couchdrop-authentication.yml
summary_line: 1 scheme
tags:
- File Transfer
- SFTP
- Automation
- Integration
- Cloud
---
