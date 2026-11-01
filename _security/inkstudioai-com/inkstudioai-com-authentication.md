---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Ink Studio AI API.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Inkstudioai Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ink Studio AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ink Studio AI
provider_slug: inkstudioai-com
scheme_count: 2
schemes:
- evidence: 'Send the key in the `Authorization` header of each request:


    ```http

    Authorization: Bearer isk_...

    ```'
  header: Authorization
  how_to_obtain: Get an API key via the CLI (`npx inkstudioai login`), the account page, or the device login flow.
  location: header
  name: Bearer
  type: http-bearer
- authorize_url: https://inkstudioai.com/cli/authorize
  evidence: The device login follows the OAuth device flow (RFC 8628).
  flows:
  - device_code
  how_to_obtain: Start the login with `POST /auth/device`, then poll `POST /auth/token` until an `apiKey` is returned.
  name: Device Login
  type: oauth2
slug: inkstudioai-com-authentication
source_filename: inkstudioai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://inkstudioai.com/developers/authentication.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://inkstudioai.com/developers/authentication.md\nsources:\n- https://inkstudioai.com/developers/authentication.md\n- https://inkstudioai.com/developers/authentication\n- https://inkstudioai.com/developers/authentication\ndescription: Authentication methods for Ink Studio AI API.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send the key in the `Authorization` header of each request:\n\n\n    ```http\n\n    Authorization: Bearer isk_...\n\n    ```'\n  location: header\n  header: Authorization\n  how_to_obtain: Get an API key via the CLI (`npx inkstudioai login`), the account page, or the device login flow.\n- type: oauth2\n  name: Device Login\n  evidence: The device login follows the OAuth device flow (RFC 8628).\n  flows:\n  - device_code\n  authorize_url: https://inkstudioai.com/cli/authorize\n  how_to_obtain: Start the login with `POST /auth/device`, then\
  \ poll `POST /auth/token` until an `apiKey` is returned.\ndocs: https://inkstudioai.com/developers/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/inkstudioai-com/authentication/inkstudioai-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Tattoo
- Design
- Generator
---
