---
anonymous_access: false
api_key_in: []
api_specs:
- filename: joinsnail-com-health-api-openapi.yml
  format: yaml
  label: SNAIL Health API
  slug: joinsnail-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsnail-com/openapi/joinsnail-com-health-api-openapi.yml
- filename: joinsnail-com-pilot-conversation-api-openapi.yml
  format: yaml
  label: SNAIL pilot conversation API
  slug: joinsnail-com-pilot-conversation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsnail-com/openapi/joinsnail-com-pilot-conversation-api-openapi.yml
- filename: joinsnail-com-platform-api-openapi.yml
  format: yaml
  label: SNAIL Platform API
  slug: joinsnail-com-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsnail-com/openapi/joinsnail-com-platform-api-openapi.yml
- filename: joinsnail-com-private-notifications-api-openapi.yml
  format: yaml
  label: SNAIL private notifications API
  slug: joinsnail-com-private-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsnail-com/openapi/joinsnail-com-private-notifications-api-openapi.yml
- filename: joinsnail-com-public-discovery-api-openapi.yml
  format: yaml
  label: SNAIL public discovery API
  slug: joinsnail-com-public-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsnail-com/openapi/joinsnail-com-public-discovery-api-openapi.yml
- filename: joinsnail-com-social-identity-api-openapi.yml
  format: yaml
  label: SNAIL social identity API
  slug: joinsnail-com-social-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsnail-com/openapi/joinsnail-com-social-identity-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: SNAIL Authentication
name_suffix: Authentication
oauth_flows: []
overview: SNAIL secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SNAIL
provider_slug: joinsnail-com
scheme_count: 1
schemes:
- name: SnailSocialCredential
  scheme: bearer
  sources:
  - openapi/joinsnail-com-openapi.yml
  type: http
slug: joinsnail-com-authentication
source_filename: joinsnail-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/joinsnail-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: SnailSocialCredential\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/joinsnail-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/joinsnail-com/authentication/joinsnail-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Agents
- Social Network
- Autonomous
- Platform
---
