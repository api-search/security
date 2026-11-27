---
anonymous_access: false
api_key_in: []
api_specs:
- filename: novence-ai-account-api-openapi.yml
  format: yaml
  label: Novence Account API
  slug: novence-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/novence-ai/openapi/novence-ai-account-api-openapi.yml
- filename: novence-ai-api-keys-api-openapi.yml
  format: yaml
  label: Novence Api Keys API
  slug: novence-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/novence-ai/openapi/novence-ai-api-keys-api-openapi.yml
- filename: novence-ai-auth-api-openapi.yml
  format: yaml
  label: Novence Auth API
  slug: novence-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/novence-ai/openapi/novence-ai-auth-api-openapi.yml
- filename: novence-ai-billing-api-openapi.yml
  format: yaml
  label: Novence Billing API
  slug: novence-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/novence-ai/openapi/novence-ai-billing-api-openapi.yml
- filename: novence-ai-bootstrap-api-openapi.yml
  format: yaml
  label: Novence Bootstrap API
  slug: novence-ai-bootstrap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/novence-ai/openapi/novence-ai-bootstrap-api-openapi.yml
- filename: novence-ai-demo-api-openapi.yml
  format: yaml
  label: Novence Demo API
  slug: novence-ai-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/novence-ai/openapi/novence-ai-demo-api-openapi.yml
- filename: novence-ai-health-api-openapi.yml
  format: yaml
  label: Novence Health API
  slug: novence-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/novence-ai/openapi/novence-ai-health-api-openapi.yml
- filename: novence-ai-invites-api-openapi.yml
  format: yaml
  label: Novence Invites API
  slug: novence-ai-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/novence-ai/openapi/novence-ai-invites-api-openapi.yml
- filename: novence-ai-llms-txt-api-openapi.yml
  format: yaml
  label: Novence Llms.txt API
  slug: novence-ai-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/novence-ai/openapi/novence-ai-llms-txt-api-openapi.yml
- filename: novence-ai-openapi-yaml-api-openapi.yml
  format: yaml
  label: Novence Openapi.yaml API
  slug: novence-ai-openapi-yaml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/novence-ai/openapi/novence-ai-openapi-yaml-api-openapi.yml
- filename: novence-ai-projects-api-openapi.yml
  format: yaml
  label: Novence Projects API
  slug: novence-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/novence-ai/openapi/novence-ai-projects-api-openapi.yml
- filename: novence-ai-public-api-openapi.yml
  format: yaml
  label: Novence Public API
  slug: novence-ai-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/novence-ai/openapi/novence-ai-public-api-openapi.yml
- filename: novence-ai-publish-html-api-openapi.yml
  format: yaml
  label: Novence Publish Html API
  slug: novence-ai-publish-html-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/novence-ai/openapi/novence-ai-publish-html-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Novence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Novence secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Novence
provider_slug: novence-ai
scheme_count: 1
schemes:
- bearerFormat: API key (nv_…) or management token (mgmt_…)
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/novence-ai-openapi.yml
  type: http
slug: novence-ai-authentication
source_filename: novence-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/novence-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key (nv_…) or management token (mgmt_…)\n  sources:\n  - openapi/novence-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/novence-ai/authentication/novence-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Hosting
- Artificial Intelligence
- Websites
- Developer Tools
---
