---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication uses Amazon Cognito. After signing in, a Cognito access token is used to call the Agents API.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Espressif Authentication
name_suffix: Authentication
oauth_flows: []
overview: Espressif Systems declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Espressif Systems
provider_slug: espressif
scheme_count: 1
schemes:
- evidence: Their access token works against the agents API too
  header: Authorization
  how_to_obtain: Sign in via Amazon Cognito (admin or end‑user sign‑up flow) to receive an access token.
  location: header
  name: Bearer
  type: http-bearer
slug: espressif-authentication
source_filename: espressif-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.agents.espressif.com/docs/deployment/authentication
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.agents.espressif.com/docs/deployment/authentication\nsources:\n- https://docs.agents.espressif.com/docs/deployment/authentication\n- https://docs.agents.espressif.com/docs/get-started/quick-start\n- https://docs.agents.espressif.com/docs/mobile_app/matter-setup\ndescription: Authentication uses Amazon Cognito. After signing in, a Cognito access token is used to call the Agents API.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Their access token works against the agents API too\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in via Amazon Cognito (admin or end‑user sign‑up flow) to receive an access token.\nnote: No explicit OAuth flow URLs or scopes are listed on the pages.\ndocs: https://docs.agents.espressif.com/docs/deployment/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/espressif/refs/heads/main/authentication/espressif-authentication.yml
summary_line: 1 scheme
tags:
- SoCs
- Modules
- Development Kits
- IoT
- AIoT
- Cloud Platform
- Wireless Connectivity
- SDK
---
