---
api_key_in: []
api_specs:
- filename: ovh-cloud-openapi-original.yml
  format: yaml
  label: OVH Cloud API
  slug: ovh-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ovh-cloud/refs/heads/main/openapi/ovh-cloud-openapi-original.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ovh Cloud Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: OVH Cloud secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: OVH Cloud
provider_slug: ovh-cloud
scheme_count: 1
schemes:
- description: Oauth2
  flows:
  - authorizationUrl: https://us.ovhcloud.com/auth/oauth2/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://us.ovhcloud.com/auth/oauth2/token
  name: oAuth2AuthCode
  sources:
  - openapi/ovh-cloud-openapi-original.yml
  type: oauth2
slug: ovh-cloud-authentication
source_filename: ovh-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ovh-cloud-openapi-original.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oAuth2AuthCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://us.ovhcloud.com/auth/oauth2/authorize\n    tokenUrl: https://us.ovhcloud.com/auth/oauth2/token\n    scopes: 3\n  description: Oauth2\n  sources:\n  - openapi/ovh-cloud-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ovh-cloud/refs/heads/main/authentication/ovh-cloud-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cloud
- Compute
- Servers
- Hosting
---
