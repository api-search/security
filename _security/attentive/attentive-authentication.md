---
api_key_in: []
api_specs:
- filename: attentive-access-token-api-openapi.yml
  format: yaml
  label: Attentive Access Token API
  slug: attentive-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-access-token-api-openapi.yml
- filename: attentive-bulk-segment-operations-api-openapi.yml
  format: yaml
  label: Attentive Bulk Segment Operations API
  slug: attentive-bulk-segment-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-bulk-segment-operations-api-openapi.yml
- filename: attentive-bulk-status-api-openapi.yml
  format: yaml
  label: Attentive Bulk Status API
  slug: attentive-bulk-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-bulk-status-api-openapi.yml
- filename: attentive-bulk-user-operations-api-openapi.yml
  format: yaml
  label: Attentive Bulk User Operations API
  slug: attentive-bulk-user-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-bulk-user-operations-api-openapi.yml
- filename: attentive-custom-attributes-api-openapi.yml
  format: yaml
  label: Attentive Custom Attributes API
  slug: attentive-custom-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-custom-attributes-api-openapi.yml
- filename: attentive-custom-events-api-openapi.yml
  format: yaml
  label: Attentive Custom Events API
  slug: attentive-custom-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-custom-events-api-openapi.yml
- filename: attentive-ecommerce-api-openapi.yml
  format: yaml
  label: Attentive eCommerce API
  slug: attentive-ecommerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-ecommerce-api-openapi.yml
- filename: attentive-identity-api-openapi.yml
  format: yaml
  label: Attentive Identity API
  slug: attentive-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-identity-api-openapi.yml
- filename: attentive-offers-api-openapi.yml
  format: yaml
  label: Attentive Offers API
  slug: attentive-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-offers-api-openapi.yml
- filename: attentive-privacy-request-api-openapi.yml
  format: yaml
  label: Attentive Privacy Request API
  slug: attentive-privacy-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-privacy-request-api-openapi.yml
- filename: attentive-product-catalog-api-openapi.yml
  format: yaml
  label: Attentive Product Catalog API
  slug: attentive-product-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-product-catalog-api-openapi.yml
- filename: attentive-segments-api-openapi.yml
  format: yaml
  label: Attentive Segments API
  slug: attentive-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-segments-api-openapi.yml
- filename: attentive-subscribers-api-openapi.yml
  format: yaml
  label: Attentive Subscribers API
  slug: attentive-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-subscribers-api-openapi.yml
- filename: attentive-test-authentication-api-openapi.yml
  format: yaml
  label: Attentive Test Authentication API
  slug: attentive-test-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-test-authentication-api-openapi.yml
- filename: attentive-test-authentication-v2-api-openapi.yml
  format: yaml
  label: Attentive Test Authentication V2 API
  slug: attentive-test-authentication-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-test-authentication-v2-api-openapi.yml
- filename: attentive-user-attributes-api-openapi.yml
  format: yaml
  label: Attentive User Attributes API
  slug: attentive-user-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-user-attributes-api-openapi.yml
- filename: attentive-user-properties-api-openapi.yml
  format: yaml
  label: Attentive User Properties API
  slug: attentive-user-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-user-properties-api-openapi.yml
- filename: attentive-webhooks-api-openapi.yml
  format: yaml
  label: Attentive Webhooks API
  slug: attentive-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Attentive Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Attentive secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Attentive
provider_slug: attentive
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/attentive-v1-openapi.yaml
  - openapi/attentive-v2-openapi.yaml
  type: http
- description: This API uses OAuth 2 with the authorization code grant flow. [More info](https://docs.attentivemobile.com/pages/authentication/)
  flows:
  - authorizationUrl: https://ui-devel.attentivemobile.com/integrations/oauth-install?client_id={clientId}&redirect_uri={redirectUri}&scope={scope}
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://api.attentivemobile.com/v1/authorization-codes/tokens
  name: OAuthFlow
  sources:
  - openapi/attentive-v1-openapi.yaml
  - openapi/attentive-v2-openapi.yaml
  type: oauth2
slug: attentive-authentication
source_filename: attentive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/attentive-v1-openapi.yaml, openapi/attentive-v2-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  - openapi/attentive-v2-openapi.yaml\n- name: OAuthFlow\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ui-devel.attentivemobile.com/integrations/oauth-install?client_id={clientId}&redirect_uri={redirectUri}&scope={scope}\n    tokenUrl: https://api.attentivemobile.com/v1/authorization-codes/tokens\n    scopes: 6\n  description: This API uses OAuth 2 with the authorization code grant flow. [More\n    info](https://docs.attentivemobile.com/pages/authentication/)\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  - openapi/attentive-v2-openapi.yaml\ndocs: https://docs.attentive.com/docs/authentication\nnotes:\
  \ Bearer token in Authorization header. Private apps use a token generated in\n  the Attentive product; public apps use OAuth 2.0 authorization code grant (code\n  expires in 2 minutes) with install at ui.attentivemobile.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/authentication/attentive-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- MarTech
- SMS Marketing
- Email Marketing
- E-Commerce
- Marketing Automation
- Subscribers
- Webhook
- Customer Engagement
---
