---
anonymous_access: false
api_key_in: []
api_specs:
- filename: justautomate-ai-agents-api-openapi.yml
  format: yaml
  label: JustAutomate Agents API
  slug: justautomate-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justautomate-ai/openapi/justautomate-ai-agents-api-openapi.yml
- filename: justautomate-ai-contact-api-openapi.yml
  format: yaml
  label: JustAutomate Contact API
  slug: justautomate-ai-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justautomate-ai/openapi/justautomate-ai-contact-api-openapi.yml
- filename: justautomate-ai-content-api-openapi.yml
  format: yaml
  label: JustAutomate Content API
  slug: justautomate-ai-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justautomate-ai/openapi/justautomate-ai-content-api-openapi.yml
- filename: justautomate-ai-meta-api-openapi.yml
  format: yaml
  label: JustAutomate Meta API
  slug: justautomate-ai-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justautomate-ai/openapi/justautomate-ai-meta-api-openapi.yml
- filename: justautomate-ai-offer-api-openapi.yml
  format: yaml
  label: JustAutomate Offer API
  slug: justautomate-ai-offer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justautomate-ai/openapi/justautomate-ai-offer-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: JustAutomate Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: JustAutomate secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: JustAutomate
provider_slug: justautomate-ai
scheme_count: 1
schemes:
- description: Optional. Identifies the agent and raises the rate limit to 600 requests per minute. Dynamic client registration and anonymous agent registration are described at https://justautomate.ai/auth.md.
  flows:
  - authorizationUrl: https://justautomate.ai/oauth/authorize/
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://justautomate.ai/oauth/token/
  name: agentOAuth
  sources:
  - openapi/justautomate-ai-openapi.json
  type: oauth2
slug: justautomate-ai-authentication
source_filename: justautomate-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/justautomate-ai-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: agentOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://justautomate.ai/oauth/authorize/\n    tokenUrl: https://justautomate.ai/oauth/token/\n    scopes: 1\n  description: Optional. Identifies the agent and raises the rate limit to 600 requests per\n    minute. Dynamic client registration and anonymous agent registration are described at https://justautomate.ai/auth.md.\n  sources:\n  - openapi/justautomate-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/justautomate-ai/authentication/justautomate-ai-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Artificial Intelligence
- Automation
- B2B
- Process Optimization
- Software-as-a-Service
- Company
---
