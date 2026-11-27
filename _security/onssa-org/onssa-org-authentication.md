---
anonymous_access: false
api_key_in: []
api_specs:
- filename: onssa-org-agent-api-openapi.yml
  format: yaml
  label: Onça Agent API
  slug: onssa-org-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onssa-org/openapi/onssa-org-agent-api-openapi.yml
- filename: onssa-org-ask-api-openapi.yml
  format: yaml
  label: Onça Ask API
  slug: onssa-org-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onssa-org/openapi/onssa-org-ask-api-openapi.yml
- filename: onssa-org-feed-api-openapi.yml
  format: yaml
  label: Onça Feed API
  slug: onssa-org-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/onssa-org/openapi/onssa-org-feed-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Onça Authentication
name_suffix: Authentication
oauth_flows: []
overview: Onça secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Onça
provider_slug: onssa-org
scheme_count: 1
schemes:
- description: A tenant API key (sk_onca_…) issued in the tenant's admin panel.
  name: tenantApiKey
  scheme: bearer
  sources:
  - openapi/onssa-org-openapi.yml
  type: http
slug: onssa-org-authentication
source_filename: onssa-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/onssa-org-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: tenantApiKey\n  type: http\n  scheme: bearer\n  description: A tenant API key (sk_onca_…) issued in the tenant's admin panel.\n  sources:\n  - openapi/onssa-org-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/onssa-org/authentication/onssa-org-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Software-as-a-Service
- Competitive Intelligence
- Brazil
- B2B
---
