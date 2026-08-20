---
api_key_in: []
api_specs:
- filename: flightcontrol-cloudfront-api-openapi.yml
  format: yaml
  label: Flightcontrol CloudFront API
  slug: flightcontrol-cloudfront-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightcontrol/refs/heads/main/openapi/flightcontrol-cloudfront-api-openapi.yml
- filename: flightcontrol-deploy-hooks-api-openapi.yml
  format: yaml
  label: Flightcontrol Deploy Hooks API
  slug: flightcontrol-deploy-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightcontrol/refs/heads/main/openapi/flightcontrol-deploy-hooks-api-openapi.yml
- filename: flightcontrol-deployments-api-openapi.yml
  format: yaml
  label: Flightcontrol Deployments API
  slug: flightcontrol-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightcontrol/refs/heads/main/openapi/flightcontrol-deployments-api-openapi.yml
- filename: flightcontrol-environment-variables-api-openapi.yml
  format: yaml
  label: Flightcontrol Environment Variables API
  slug: flightcontrol-environment-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightcontrol/refs/heads/main/openapi/flightcontrol-environment-variables-api-openapi.yml
- filename: flightcontrol-environments-api-openapi.yml
  format: yaml
  label: Flightcontrol Environments API
  slug: flightcontrol-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightcontrol/refs/heads/main/openapi/flightcontrol-environments-api-openapi.yml
- filename: flightcontrol-services-api-openapi.yml
  format: yaml
  label: Flightcontrol Services API
  slug: flightcontrol-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flightcontrol/refs/heads/main/openapi/flightcontrol-services-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Flightcontrol Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flightcontrol secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flightcontrol
provider_slug: flightcontrol
scheme_count: 1
schemes:
- description: Flightcontrol API key passed as a Bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/flightcontrol-openapi.yml
  type: http
slug: flightcontrol-authentication
source_filename: flightcontrol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flightcontrol-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Flightcontrol API key passed as a Bearer token in the Authorization header.\n  sources:\n  - openapi/flightcontrol-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flightcontrol/refs/heads/main/authentication/flightcontrol-authentication.yml
summary_line: http · 1 scheme
tags:
- Deployment
- Platform-as-a-Service
- Infrastructure
- DevOps
---
