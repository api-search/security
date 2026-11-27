---
anonymous_access: false
api_key_in: []
api_specs:
- filename: m2msentinel-com-capabilities-api-openapi.yml
  format: yaml
  label: M2M Sentinel Capabilities API
  slug: m2msentinel-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/m2msentinel-com/openapi/m2msentinel-com-capabilities-api-openapi.yml
- filename: m2msentinel-com-demo-api-openapi.yml
  format: yaml
  label: M2M Sentinel Demo API
  slug: m2msentinel-com-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/m2msentinel-com/openapi/m2msentinel-com-demo-api-openapi.yml
- filename: m2msentinel-com-keys-api-openapi.yml
  format: yaml
  label: M2M Sentinel Keys API
  slug: m2msentinel-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/m2msentinel-com/openapi/m2msentinel-com-keys-api-openapi.yml
- filename: m2msentinel-com-market-api-openapi.yml
  format: yaml
  label: M2M Sentinel Market API
  slug: m2msentinel-com-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/m2msentinel-com/openapi/m2msentinel-com-market-api-openapi.yml
- filename: m2msentinel-com-mcp-api-openapi.yml
  format: yaml
  label: M2M Sentinel MCP API
  slug: m2msentinel-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/m2msentinel-com/openapi/m2msentinel-com-mcp-api-openapi.yml
- filename: m2msentinel-com-onboarding-api-openapi.yml
  format: yaml
  label: M2M Sentinel Onboarding API
  slug: m2msentinel-com-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/m2msentinel-com/openapi/m2msentinel-com-onboarding-api-openapi.yml
- filename: m2msentinel-com-operator-api-openapi.yml
  format: yaml
  label: M2M Sentinel Operator API
  slug: m2msentinel-com-operator-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/m2msentinel-com/openapi/m2msentinel-com-operator-api-openapi.yml
- filename: m2msentinel-com-status-api-openapi.yml
  format: yaml
  label: M2M Sentinel Status API
  slug: m2msentinel-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/m2msentinel-com/openapi/m2msentinel-com-status-api-openapi.yml
auth_types: []
description: Authentication uses an API key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: M2M Sentinel Authentication
name_suffix: Authentication
oauth_flows: []
overview: M2M Sentinel declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: M2M Sentinel
provider_slug: m2msentinel-com
scheme_count: 1
schemes:
- evidence: The key is sent in the x-api-key header only.
  header: x-api-key
  how_to_obtain: Claim a free key or purchase a paid key via wallet signature; the server issues the key after signing a challenge.
  location: header
  name: API Key
  type: apiKey
slug: m2msentinel-com-authentication
source_filename: m2msentinel-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.m2msentinel.com/api_keys.html
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.m2msentinel.com/api_keys.html\nsources:\n- https://www.m2msentinel.com/api_keys.html\n- https://www.m2msentinel.com/api_keys.html\n- https://www.m2msentinel.com/inspector.html\ndescription: Authentication uses an API key.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: The key is sent in the x-api-key header only.\n  location: header\n  header: x-api-key\n  how_to_obtain: Claim a free key or purchase a paid key via wallet signature; the server issues the key after signing a challenge.\nnote: No OAuth2, HTTP Bearer, HTTP Basic, JWT, HMAC, MTLS, or other schemes are documented on the provided pages.\ndocs: https://www.m2msentinel.com/api_keys.html\n"
source_yaml_url: https://artifacts.apis.io/m2msentinel-com/authentication/m2msentinel-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Integration
- JavaScript
- TypeScript
- Blockchain
---
