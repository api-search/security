---
anonymous_access: false
api_key_in: []
api_specs:
- filename: intermind-com-openapi-generated.yml
  format: yaml
  label: InterMIND API
  slug: intermind-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intermind-com/openapi/_ae-authored/intermind-com-openapi-generated.yml
auth_types: []
description: InterMIND API authentication uses a personal API key sent as a bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: InterMIND Authentication
name_suffix: Authentication
oauth_flows: []
overview: InterMIND declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: InterMIND
provider_slug: intermind-com
scheme_count: 1
schemes:
- evidence: 'Send the key as a bearer token: Authorization: Bearer imk_…'
  header: Authorization
  how_to_obtain: Create a key in Integrations → API keys, copy the key that starts with imk_.
  location: header
  name: API key
  type: http-bearer
slug: intermind-com-authentication
source_filename: intermind-com-authentication.yml
source_heading: Authentication Profile
source_url: https://intermind.com/docs/integrations/api-zapier
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://intermind.com/docs/integrations/api-zapier\nsources:\n- https://intermind.com/docs/integrations/api-zapier\n- https://intermind.com/raw/docs/getting-started/sign-in.md\n- https://intermind.com/docs/getting-started/sign-in\n- https://intermind.com/raw/blog/email-to-channel-no-bot.md\ndescription: InterMIND API authentication uses a personal API key sent as a bearer token.\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Send the key as a bearer token: Authorization: Bearer imk_…'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Integrations → API keys, copy the key that starts with imk_.\ndocs: https://intermind.com/docs/integrations/api-zapier\n"
source_yaml_url: https://artifacts.apis.io/intermind-com/authentication/intermind-com-authentication.yml
summary_line: 1 scheme
tags:
- Collaboration
- Multilingual
- Artificial Intelligence
- Real-Time Translation
- Distributed-team
---
