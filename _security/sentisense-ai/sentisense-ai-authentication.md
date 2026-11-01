---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sentisense-ai-openapi-generated.yml
  format: yaml
  label: sentisense-ai API
  slug: sentisense-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sentisense-ai/openapi/_ae-authored/sentisense-ai-openapi-generated.yml
auth_types: []
description: Authentication schemes for SentiSense API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Sentisense Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: sentisense-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: sentisense-ai
provider_slug: sentisense-ai
scheme_count: 1
schemes:
- evidence: 'Authentication: no API key needed. This is the one endpoint that takes no key; every call made with the key it returns sends it in the X‑SentiSense‑API‑Key header as usual.'
  header: X-SentiSense-API-Key
  how_to_obtain: Returned in the response of POST /api/v1/keys/provision
  location: header
  name: API Key
  type: apiKey
slug: sentisense-ai-authentication
source_filename: sentisense-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://sentisense.ai/docs/api/keys/
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://sentisense.ai/docs/api/keys/\nsources:\n- https://sentisense.ai/docs/api/keys/\n- https://sentisense.ai/docs/api/keys/\n- https://sentisense.ai/docs/api/connectors/\n- https://sentisense.ai/docs/api/keys.md\ndescription: Authentication schemes for SentiSense API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Authentication: no API key needed. This is the one endpoint that takes no key; every call made with the key it returns sends it in\n    the X‑SentiSense‑API‑Key header as usual.'\n  location: header\n  header: X-SentiSense-API-Key\n  how_to_obtain: Returned in the response of POST /api/v1/keys/provision\ndocs: https://sentisense.ai/docs/api/keys/\n"
source_yaml_url: https://artifacts.apis.io/sentisense-ai/authentication/sentisense-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Analytics
- Machine-Learning
- Enterprise
---
