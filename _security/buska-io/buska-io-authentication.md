---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods documented for Buska API and its integrations.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Buska Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buska declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Buska
provider_slug: buska-io
scheme_count: 1
schemes:
- evidence: All API requests require an API key passed in the x-api-key header.
  header: x-api-key
  how_to_obtain: Go to Settings > API in the Buska dashboard, click "Generate API Key", copy the key and store it securely.
  location: header
  name: API Key
  type: apiKey
slug: buska-io-authentication
source_filename: buska-io-authentication.yml
source_heading: Authentication Profile
source_url: https://www.buska.io/docs/api/authentication
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.buska.io/docs/api/authentication\nsources:\n- https://www.buska.io/docs/api/authentication\n- https://www.buska.io/docs/integrations/hubspot\n- https://www.buska.io/docs/integrations/salesforce\n- https://www.buska.io/docs/integrations/pipedrive\ndescription: Authentication methods documented for Buska API and its integrations.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: All API requests require an API key passed in the x-api-key header.\n  location: header\n  header: x-api-key\n  how_to_obtain: Go to Settings > API in the Buska dashboard, click \"Generate API Key\", copy the key and store it securely.\ndocs: https://www.buska.io/docs/api/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/buska-io/authentication/buska-io-authentication.yml
summary_line: 1 scheme
tags:
- Social Listening
- Lead Generation
- Artificial Intelligence
- B2B
- Marketing
---
