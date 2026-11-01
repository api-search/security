---
anonymous_access: false
api_key_in: []
auth_types: []
description: Requests using XM-Serve require a NETPREME_API_KEY.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Netpreme Authentication
name_suffix: Authentication
oauth_flows: []
overview: Netpreme declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Netpreme
provider_slug: netpreme
scheme_count: 1
schemes:
- evidence: Requests using XM-Serve require a NETPREME_API_KEY .
  header: Authorization
  how_to_obtain: Register an account at api.netpreme.com, create a key under API Keys, and save the key.
  location: header
  name: API Key
  type: apiKey
slug: netpreme-authentication
source_filename: netpreme-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.netpreme.com/quickstart/
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.netpreme.com/quickstart/\nsources:\n- https://docs.netpreme.com/quickstart/\ndescription: Requests using XM-Serve require a NETPREME_API_KEY.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Requests using XM-Serve require a NETPREME_API_KEY .\n  location: header\n  header: Authorization\n  how_to_obtain: Register an account at api.netpreme.com, create a key under API Keys, and save the key.\nnote: No OAuth2 or other authentication schemes are documented on the page.\ndocs: https://docs.netpreme.com/quickstart/\n"
source_yaml_url: https://artifacts.apis.io/netpreme/authentication/netpreme-authentication.yml
summary_line: 1 scheme
tags:
- Memory Systems
- AI Compute
- MPU
- Inference Hardware
- GPU Memory
- Silicon
---
