---
api_key_in:
- header
api_specs:
- filename: whatfix-openapi.yml
  format: yaml
  label: Whatfix REST API
  slug: whatfix-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/whatfix/refs/heads/main/openapi/whatfix-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Whatfix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Whatfix secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Whatfix
provider_slug: whatfix
scheme_count: 1
schemes:
- description: User API token obtained from the Whatfix dashboard. Pass your registered Whatfix email address in the x-whatfix-user header as well.
  in: header
  name: ApiKeyAuth
  parameter: x-whatfix-integration-key
  sources:
  - openapi/whatfix-openapi.yml
  type: apiKey
slug: whatfix-authentication
source_filename: whatfix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/whatfix-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-whatfix-integration-key\n  description: User API token obtained from the Whatfix dashboard. Pass your registered Whatfix\n    email address in the x-whatfix-user header as well.\n  sources:\n  - openapi/whatfix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whatfix/refs/heads/main/authentication/whatfix-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Digital Adoption
- In-App Guidance
- Onboarding
- Analytics
- Self-Help
---
