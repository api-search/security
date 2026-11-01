---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cybermaxtools-com-namewhere-api-openapi.yml
  format: yaml
  label: cybermaxtools-com Namewhere API
  slug: cybermaxtools-com-namewhere-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cybermaxtools-com/openapi/cybermaxtools-com-namewhere-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cybermaxtools Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: cybermaxtools-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: cybermaxtools-com
provider_slug: cybermaxtools-com
scheme_count: 2
schemes:
- description: Optional. Paid plan key from https://namewhere.cybermaxtools.com/docs#pricing; leave out for the free tier.
  in: header
  name: x-api-key
  type: apiKey
- description: Same key as a Bearer token.
  scheme: bearer
  type: http
slug: cybermaxtools-com-authentication
source_filename: cybermaxtools-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: searched\nsource: https://namewhere.cybermaxtools.com/openapi.json\nschemes:\n  - type: apiKey\n    name: x-api-key\n    in: header\n    description: Optional. Paid plan key from https://namewhere.cybermaxtools.com/docs#pricing; leave out for the free tier.\n  - type: http\n    scheme: bearer\n    description: Same key as a Bearer token.\n"
source_yaml_url: https://artifacts.apis.io/cybermaxtools-com/authentication/cybermaxtools-com-authentication.yml
summary_line: 2 schemes
tags:
- Games
- AI
- Data APIs
- Creator Kits
- Marketplace
---
