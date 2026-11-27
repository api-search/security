---
anonymous_access: false
api_key_in: []
api_specs:
- filename: formasty-com-capabilities-api-openapi.yml
  format: yaml
  label: Formasty Capabilities API
  slug: formasty-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formasty-com/openapi/formasty-com-capabilities-api-openapi.yml
- filename: formasty-com-forms-api-openapi.yml
  format: yaml
  label: Formasty Forms API
  slug: formasty-com-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formasty-com/openapi/formasty-com-forms-api-openapi.yml
- filename: formasty-com-me-api-openapi.yml
  format: yaml
  label: Formasty Me API
  slug: formasty-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/formasty-com/openapi/formasty-com-me-api-openapi.yml
auth_types: []
description: Authentication schemes published on Formasty documentation
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Formasty Authentication
name_suffix: Authentication
oauth_flows: []
overview: Formasty declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Formasty
provider_slug: formasty-com
scheme_count: 1
schemes:
- evidence: 'Authenticate every request with a Bearer token. Create a key Workspace → API keys. Click Create API key. Name it. Pick scopes. Copy the key (shown once). It looks like: formasty_xxx… Send it on every request as Authorization: Bearer YOUR_KEY.'
  header: Authorization
  how_to_obtain: Create an API key in the Formasty workspace under API keys and copy the generated key.
  location: header
  name: Bearer
  type: http-bearer
slug: formasty-com-authentication
source_filename: formasty-com-authentication.yml
source_heading: Authentication Profile
source_url: https://formasty.com/documentation/api-auth
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://formasty.com/documentation/api-auth\nsources:\n- https://formasty.com/documentation/api-auth\n- https://formasty.com/mcp-form-builder\ndescription: Authentication schemes published on Formasty documentation\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authenticate every request with a Bearer token. Create a key Workspace → API keys. Click Create API key. Name it. Pick scopes. Copy\n    the key (shown once). It looks like: formasty_xxx… Send it on every request as Authorization: Bearer YOUR_KEY.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the Formasty workspace under API keys and copy the generated key.\ndocs: https://formasty.com/documentation/api-auth\n"
source_yaml_url: https://artifacts.apis.io/formasty-com/authentication/formasty-com-authentication.yml
summary_line: 1 scheme
tags:
- Lead Qualification
- Forms
- Artificial Intelligence
- Automation
- Software-as-a-Service
---
