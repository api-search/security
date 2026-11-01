---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses an API key passed in a header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hatchloop Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: hatchloop-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: hatchloop-dev
provider_slug: hatchloop-dev
scheme_count: 1
schemes:
- evidence: Pass your key as the X-Agent-Identity header.
  header: X-Agent-Identity
  how_to_obtain: Request a free key by submitting your email via POST https://hatchloop.dev/keys/request and clicking the verification link sent to your inbox.
  location: header
  name: X-Agent-Identity
  type: apiKey
slug: hatchloop-dev-authentication
source_filename: hatchloop-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://hatchloop.dev/docs/#auth
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hatchloop.dev/docs/#auth\nsources:\n- https://hatchloop.dev/docs/#auth\n- https://hatchloop.dev/docs/\ndescription: Authentication uses an API key passed in a header.\nschemes:\n- type: apiKey\n  name: X-Agent-Identity\n  evidence: Pass your key as the X-Agent-Identity header.\n  location: header\n  header: X-Agent-Identity\n  how_to_obtain: Request a free key by submitting your email via POST https://hatchloop.dev/keys/request and clicking the verification link sent\n    to your inbox.\nnote: No other authentication methods (OAuth, http-bearer, etc.) are documented on the provided pages.\ndocs: https://hatchloop.dev/docs/#auth\n"
source_yaml_url: https://artifacts.apis.io/hatchloop-dev/authentication/hatchloop-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Automation
- API
- Platform
- DeveloperTools
---
