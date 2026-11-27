---
anonymous_access: false
api_key_in: []
api_specs:
- filename: manyscripts-com-openapi-generated.yml
  format: yaml
  label: ManyScripts API
  slug: manyscripts-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/manyscripts-com/openapi/_ae-authored/manyscripts-com-openapi-generated.yml
auth_types: []
description: Authentication uses an API key provided as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ManyScripts Authentication
name_suffix: Authentication
oauth_flows: []
overview: ManyScripts declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ManyScripts
provider_slug: manyscripts-com
scheme_count: 1
schemes:
- evidence: 'Open the Dashboard and choose the Connect & Integrations tab to create a key, then POST {"url": "<public video URL>"} as JSON to https://www.manyscripts.com/api/v1/transcript with Authorization: Bearer msk_your_key.'
  header: Authorization
  how_to_obtain: Create an API key in the ManyScripts Dashboard under Connect & Integrations; the key starts with "msk_".
  location: header
  name: Bearer token
  type: http-bearer
slug: manyscripts-com-authentication
source_filename: manyscripts-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.manyscripts.com/docs/api-quickstart
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.manyscripts.com/docs/api-quickstart\nsources:\n- https://www.manyscripts.com/docs/api-quickstart\ndescription: Authentication uses an API key provided as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Open the Dashboard and choose the Connect & Integrations tab to create a key, then POST {\"url\": \"<public video URL>\"} as JSON to\n    https://www.manyscripts.com/api/v1/transcript with Authorization: Bearer msk_your_key.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the ManyScripts Dashboard under Connect & Integrations; the key starts with \"msk_\".\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the page.\ndocs: https://www.manyscripts.com/docs/api-quickstart\n"
source_yaml_url: https://artifacts.apis.io/manyscripts-com/authentication/manyscripts-com-authentication.yml
summary_line: 1 scheme
tags:
- Transcription
- Video
- Artificial Intelligence
- Creator Tools
- Marketing
---
