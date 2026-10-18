---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Lytix
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Lytix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lytix declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lytix
provider_slug: lytix
scheme_count: 1
schemes:
- evidence: All Lytix SDKs use the `LX_API_KEY` environment variable to authenticate with the Lytix platform.
  how_to_obtain: Create an API key in the Lytix platform Settings → API Keys page and copy it.
  name: API Key
  type: apiKey
slug: lytix-authentication
source_filename: lytix-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.lytix.co/APIKeys/api-key-setup.md
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.lytix.co/APIKeys/api-key-setup.md\nsources:\n- https://docs.lytix.co/APIKeys/api-key-setup.md\n- https://docs.lytix.co/APIKeys/set-api-key-in-code.md\n- https://docs.lytix.co/APIKeys/api-keys-and-workflows.md\n- https://docs.lytix.co/APIKeys/env-var-setup.md\ndescription: Authentication schemes for Lytix\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: All Lytix SDKs use the `LX_API_KEY` environment variable to authenticate with the Lytix platform.\n  how_to_obtain: Create an API key in the Lytix platform Settings → API Keys page and copy it.\ndocs: https://docs.lytix.co/APIKeys/api-key-setup.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lytix/refs/heads/main/authentication/lytix-authentication.yml
summary_line: 1 scheme
tags:
- AI
- LLMOps
- Evaluation
- Monitoring
- OpenSource
---
