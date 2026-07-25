---
api_key_in: []
api_specs:
- filename: motion-elements-account-api-openapi.yml
  format: yaml
  label: Motion Elements Account API
  slug: motion-elements-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/motion-elements/refs/heads/main/openapi/motion-elements-account-api-openapi.yml
- filename: motion-elements-elements-api-openapi.yml
  format: yaml
  label: Motion Elements Elements API
  slug: motion-elements-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/motion-elements/refs/heads/main/openapi/motion-elements-elements-api-openapi.yml
- filename: motion-elements-media-types-api-openapi.yml
  format: yaml
  label: Motion Elements Media types API
  slug: motion-elements-media-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/motion-elements/refs/heads/main/openapi/motion-elements-media-types-api-openapi.yml
- filename: motion-elements-search-api-openapi.yml
  format: yaml
  label: Motion Elements Search API
  slug: motion-elements-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/motion-elements/refs/heads/main/openapi/motion-elements-search-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Motion Elements Authentication
name_suffix: Authentication
oauth_flows: []
overview: Motion Elements secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Motion Elements
provider_slug: motion-elements
scheme_count: 1
schemes:
- description: HTTP Basic authentication. Use your API secret key (created in the Developer Console) as the username; leave the password empty.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/motion-elements-openapi.yml
  type: http
slug: motion-elements-authentication
source_filename: motion-elements-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/motion-elements-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Use your API secret key (created in the Developer\n    Console) as the username; leave the password empty.\n  sources:\n  - openapi/motion-elements-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motion-elements/refs/heads/main/authentication/motion-elements-authentication.yml
summary_line: http · 1 scheme
tags:
- Media
- Stock Media
- Video
- Music
- Sound Effects
- Templates
- Marketplace
- Creative Assets
- Generative AI
- Search
- Company
---
