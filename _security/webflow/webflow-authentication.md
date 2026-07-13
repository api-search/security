---
api_key_in: []
api_specs:
- filename: webflow-data-api-openapi.yml
  format: yaml
  label: Webflow Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-data-api-openapi.yml
- filename: webflow-meta-openapi.yml
  format: yaml
  label: Webflow Meta API
  slug: meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-meta-openapi.yml
- filename: webflow-sites-openapi.yml
  format: yaml
  label: Webflow Sites API
  slug: sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-sites-openapi.yml
- filename: webflow-pages-openapi.yml
  format: yaml
  label: Webflow Pages API
  slug: pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-pages-openapi.yml
- filename: webflow-collections-openapi.yml
  format: yaml
  label: Webflow Collections API
  slug: collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-collections-openapi.yml
- filename: webflow-items-openapi.yml
  format: yaml
  label: Webflow CMS Items API
  slug: items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-items-openapi.yml
- filename: webflow-components-openapi.yml
  format: yaml
  label: Webflow Components API
  slug: components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-components-openapi.yml
- filename: webflow-assets-openapi.yml
  format: yaml
  label: Webflow Assets API
  slug: assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-assets-openapi.yml
- filename: webflow-forms-openapi.yml
  format: yaml
  label: Webflow Forms API
  slug: forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-forms-openapi.yml
- filename: webflow-products-openapi.yml
  format: yaml
  label: Webflow Products and SKUs API
  slug: products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-products-openapi.yml
- filename: webflow-orders-openapi.yml
  format: yaml
  label: Webflow Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-orders-openapi.yml
- filename: webflow-inventory-openapi.yml
  format: yaml
  label: Webflow Inventory API
  slug: inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-inventory-openapi.yml
- filename: webflow-ecommerce-settings-openapi.yml
  format: yaml
  label: Webflow Ecommerce Settings API
  slug: ecommerce-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-ecommerce-settings-openapi.yml
- filename: webflow-webhooks-openapi.yml
  format: yaml
  label: Webflow Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-webhooks-openapi.yml
- filename: webflow-custom-code-openapi.yml
  format: yaml
  label: Webflow Custom Code API
  slug: custom-code-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-custom-code-openapi.yml
- filename: webflow-comments-openapi.yml
  format: yaml
  label: Webflow Comments API
  slug: comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/openapi/webflow-comments-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Webflow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Webflow secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Webflow
provider_slug: webflow
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://webflow.com/oauth/authorize
    flow: authorizationCode
    scopes: 26
    tokenUrl: https://api.webflow.com/oauth/token
  name: OAuth2
  sources:
  - openapi/webflow-assets-openapi.yml
  - openapi/webflow-collections-openapi.yml
  - openapi/webflow-comments-openapi.yml
  - openapi/webflow-components-openapi.yml
  - openapi/webflow-custom-code-openapi.yml
  - openapi/webflow-data-api-openapi.yml
  - openapi/webflow-ecommerce-settings-openapi.yml
  - openapi/webflow-forms-openapi.yml
  - openapi/webflow-inventory-openapi.yml
  - openapi/webflow-items-openapi.yml
  - openapi/webflow-meta-openapi.yml
  - openapi/webflow-orders-openapi.yml
  - openapi/webflow-pages-openapi.yml
  - openapi/webflow-products-openapi.yml
  - openapi/webflow-sites-openapi.yml
  - openapi/webflow-webhooks-openapi.yml
  type: oauth2
- name: ApiKey
  scheme: bearer
  sources:
  - openapi/webflow-assets-openapi.yml
  - openapi/webflow-collections-openapi.yml
  - openapi/webflow-comments-openapi.yml
  - openapi/webflow-components-openapi.yml
  - openapi/webflow-custom-code-openapi.yml
  - openapi/webflow-data-api-openapi.yml
  - openapi/webflow-ecommerce-settings-openapi.yml
  - openapi/webflow-forms-openapi.yml
  - openapi/webflow-inventory-openapi.yml
  - openapi/webflow-items-openapi.yml
  - openapi/webflow-meta-openapi.yml
  - openapi/webflow-orders-openapi.yml
  - openapi/webflow-pages-openapi.yml
  - openapi/webflow-products-openapi.yml
  - openapi/webflow-sites-openapi.yml
  - openapi/webflow-webhooks-openapi.yml
  type: http
slug: webflow-authentication
source_filename: webflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/webflow-assets-openapi.yml, openapi/webflow-collections-openapi.yml, openapi/webflow-comments-openapi.yml,\n  openapi/webflow-components-openapi.yml, openapi/webflow-custom-code-openapi.yml, openapi/webflow-data-api-openapi.yml,\n  openapi/webflow-ecommerce-settings-openapi.yml, openapi/webflow-forms-openapi.yml, openapi/webflow-inventory-openapi.yml,\n  openapi/webflow-items-openapi.yml, openapi/webflow-meta-openapi.yml, openapi/webflow-orders-openapi.yml\n  ...\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://webflow.com/oauth/authorize\n    tokenUrl: https://api.webflow.com/oauth/token\n    scopes: 26\n  sources:\n  - openapi/webflow-assets-openapi.yml\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-comments-openapi.yml\n  - openapi/webflow-components-openapi.yml\n\
  \  - openapi/webflow-custom-code-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-ecommerce-settings-openapi.yml\n  - openapi/webflow-forms-openapi.yml\n  - openapi/webflow-inventory-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-meta-openapi.yml\n  - openapi/webflow-orders-openapi.yml\n  - openapi/webflow-pages-openapi.yml\n  - openapi/webflow-products-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n- name: ApiKey\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/webflow-assets-openapi.yml\n  - openapi/webflow-collections-openapi.yml\n  - openapi/webflow-comments-openapi.yml\n  - openapi/webflow-components-openapi.yml\n  - openapi/webflow-custom-code-openapi.yml\n  - openapi/webflow-data-api-openapi.yml\n  - openapi/webflow-ecommerce-settings-openapi.yml\n  - openapi/webflow-forms-openapi.yml\n  - openapi/webflow-inventory-openapi.yml\n  - openapi/webflow-items-openapi.yml\n  - openapi/webflow-meta-openapi.yml\n\
  \  - openapi/webflow-orders-openapi.yml\n  - openapi/webflow-pages-openapi.yml\n  - openapi/webflow-products-openapi.yml\n  - openapi/webflow-sites-openapi.yml\n  - openapi/webflow-webhooks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webflow/refs/heads/main/authentication/webflow-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- CMS
- Ecommerce
- No-Code
- Web Development
---
