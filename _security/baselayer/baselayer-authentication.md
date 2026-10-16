---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods published on the Baselayer documentation pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Baselayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Baselayer declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Baselayer
provider_slug: baselayer
scheme_count: 1
schemes:
- evidence: All Baselayer API requests require authentication using an API key passed in the `X-API-Key` header.
  header: X-API-Key
  how_to_obtain: Log into the Baselayer console, navigate to the API Keys section, and copy your API key.
  location: header
  name: API Key
  type: apiKey
slug: baselayer-authentication
source_filename: baselayer-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.baselayer.com/docs/authentication.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.baselayer.com/docs/authentication.md\nsources:\n- https://docs.baselayer.com/docs/authentication.md\n- https://docs.baselayer.com/api-reference/platform/api-key-created.md\n- https://docs.baselayer.com/api-reference/platform/api-key-deleted.md\n- https://docs.baselayer.com/changelog/mcp-api-key-authentication-and-international-tools.md\ndescription: Authentication methods published on the Baselayer documentation pages.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: All Baselayer API requests require authentication using an API key passed in the `X-API-Key` header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Log into the Baselayer console, navigate to the API Keys section, and copy your API key.\nnote: The documentation also describes HMAC‑SHA256 signatures for webhook verification, which is not a client authentication scheme for API requests.\n\
  docs: https://docs.baselayer.com/docs/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baselayer/refs/heads/main/authentication/baselayer-authentication.yml
summary_line: 1 scheme
tags:
- Business
- IdentityVerification
- RiskManagement
- FinTech
- API
---
