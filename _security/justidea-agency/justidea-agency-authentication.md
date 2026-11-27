---
anonymous_access: false
api_key_in: []
api_specs:
- filename: justidea-agency-agents-api-openapi.yml
  format: yaml
  label: JustIdea Agents API
  slug: justidea-agency-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justidea-agency/openapi/justidea-agency-agents-api-openapi.yml
- filename: justidea-agency-contact-api-openapi.yml
  format: yaml
  label: JustIdea Contact API
  slug: justidea-agency-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justidea-agency/openapi/justidea-agency-contact-api-openapi.yml
- filename: justidea-agency-content-api-openapi.yml
  format: yaml
  label: JustIdea Content API
  slug: justidea-agency-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justidea-agency/openapi/justidea-agency-content-api-openapi.yml
- filename: justidea-agency-meta-api-openapi.yml
  format: yaml
  label: JustIdea Meta API
  slug: justidea-agency-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justidea-agency/openapi/justidea-agency-meta-api-openapi.yml
- filename: justidea-agency-offer-api-openapi.yml
  format: yaml
  label: JustIdea Offer API
  slug: justidea-agency-offer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justidea-agency/openapi/justidea-agency-offer-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: JustIdea Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: JustIdea secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: JustIdea
provider_slug: justidea-agency
scheme_count: 1
schemes:
- description: Optional. Identifies the agent and raises the rate limit to 600 requests per minute. Dynamic client registration and anonymous agent registration are described at https://justidea.agency/auth.md.
  flows:
  - authorizationUrl: https://justidea.agency/oauth/authorize/
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://justidea.agency/oauth/token/
  name: agentOAuth
  sources:
  - openapi/justidea-agency-openapi.json
  - openapi/justidea-agency-openapi.yml
  type: oauth2
slug: justidea-agency-authentication
source_filename: justidea-agency-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/justidea-agency-openapi.json, openapi/justidea-agency-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: agentOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://justidea.agency/oauth/authorize/\n    tokenUrl: https://justidea.agency/oauth/token/\n    scopes: 1\n  description: Optional. Identifies the agent and raises the rate limit to 600 requests per\n    minute. Dynamic client registration and anonymous agent registration are described at https://justidea.agency/auth.md.\n  sources:\n  - openapi/justidea-agency-openapi.json\n  - openapi/justidea-agency-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/justidea-agency/authentication/justidea-agency-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- E-Commerce
- Agency
- Poland
- PrestaShop
- WooCommerce
---
