---
anonymous_access: false
api_key_in: []
api_specs:
- filename: goveda-com-openapi-generated.yml
  format: yaml
  label: GoVeda API
  slug: goveda-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/goveda-com/openapi/_ae-authored/goveda-com-openapi-generated.yml
auth_types: []
description: GoVeda uses API keys for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: GoVeda Authentication
name_suffix: Authentication
oauth_flows: []
overview: GoVeda declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GoVeda
provider_slug: goveda-com
scheme_count: 1
schemes:
- evidence: Pass the key in the X-API-Key request header.
  header: X-API-Key
  how_to_obtain: Create a key in GoVeda API keys settings and copy the full key value.
  location: header
  name: X-API-Key
  type: apiKey
slug: goveda-com-authentication
source_filename: goveda-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.goveda.com/en/docs/api/api-keys
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.goveda.com/en/docs/api/api-keys\nsources:\n- https://www.goveda.com/en/docs/api/api-keys\n- https://www.goveda.com/en/docs/goveda-agent/models/model-api-keys\n- https://www.goveda.com/en/docs/api/api-keys\n- https://www.goveda.com/en/docs/api\ndescription: GoVeda uses API keys for authentication.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: Pass the key in the X-API-Key request header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a key in GoVeda API keys settings and copy the full key value.\nnote: No OAuth2, HTTP basic, bearer, JWT, HMAC, or mTLS schemes are documented.\ndocs: https://www.goveda.com/en/docs/api/api-keys\n"
source_yaml_url: https://artifacts.apis.io/goveda-com/authentication/goveda-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Innovation
- Research
- Market Analysis
- Reporting
---
