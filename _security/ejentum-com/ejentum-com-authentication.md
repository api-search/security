---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Ejentum API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ejentum Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ejentum-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ejentum-com
provider_slug: ejentum-com
scheme_count: 1
schemes:
- evidence: 'Export your key in your shell or `.env` file (or pass api_key="..." directly when initializing): export EJENTUM_API_KEY=" ej_live_... "'
  header: Authorization
  how_to_obtain: Generate a $0 Free Trial key (100 req/day) or subscribe at $9/mo.
  location: header
  name: Ejentum API Key
  type: http-bearer
slug: ejentum-com-authentication
source_filename: ejentum-com-authentication.yml
source_heading: Authentication Profile
source_url: https://ejentum.com/docs/quickstart
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ejentum.com/docs/quickstart\nsources:\n- https://ejentum.com/docs/quickstart\ndescription: Authentication methods for Ejentum API\nschemes:\n- type: http-bearer\n  name: Ejentum API Key\n  evidence: 'Export your key in your shell or `.env` file (or pass api_key=\"...\" directly when initializing): export EJENTUM_API_KEY=\" ej_live_...\n    \"'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a $0 Free Trial key (100 req/day) or subscribe at $9/mo.\nnote: No OAuth2, apiKey query/body, or other authentication schemes are documented on the page.\ndocs: https://ejentum.com/docs/quickstart\n"
source_yaml_url: https://artifacts.apis.io/ejentum-com/authentication/ejentum-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Reasoning
- Agentic
- Verification
- Platform
---
