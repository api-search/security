---
api_key_in:
- header
api_specs:
- filename: contentstack-content-delivery-api-openapi.yml
  format: yaml
  label: Contentstack Content Delivery API
  slug: content-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-content-delivery-api-openapi.yml
- filename: contentstack-content-management-api-openapi.yml
  format: yaml
  label: Contentstack Content Management API
  slug: content-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-content-management-api-openapi.yml
- filename: contentstack-personalize-management-api-openapi.yml
  format: yaml
  label: Contentstack Personalize Management API
  slug: personalize-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-personalize-management-api-openapi.yml
- filename: contentstack-personalize-edge-api-openapi.yml
  format: yaml
  label: Contentstack Personalize Edge API
  slug: personalize-edge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-personalize-edge-api-openapi.yml
- filename: contentstack-automate-management-api-openapi.yml
  format: yaml
  label: Contentstack Automate Management API
  slug: automate-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-automate-management-api-openapi.yml
- filename: contentstack-analytics-api-openapi.yml
  format: yaml
  label: Contentstack Analytics API
  slug: analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-analytics-api-openapi.yml
- filename: contentstack-scim-api-openapi.yml
  format: yaml
  label: Contentstack SCIM API
  slug: scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-scim-api-openapi.yml
- filename: contentstack-brand-kit-management-api-openapi.yml
  format: yaml
  label: Contentstack Brand Kit Management API
  slug: brand-kit-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-brand-kit-management-api-openapi.yml
- filename: contentstack-knowledge-vault-api-openapi.yml
  format: yaml
  label: Contentstack Knowledge Vault API
  slug: knowledge-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-knowledge-vault-api-openapi.yml
- filename: contentstack-generative-ai-api-openapi.yml
  format: yaml
  label: Contentstack Generative AI API
  slug: generative-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-generative-ai-api-openapi.yml
- filename: contentstack-launch-api-openapi.yml
  format: yaml
  label: Contentstack Launch API
  slug: launch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/openapi/contentstack-launch-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Contentstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: contentstack secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: contentstack
provider_slug: contentstack
scheme_count: 5
schemes:
- description: OAuth 2.0 Bearer token (M2M) with analytics access.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/contentstack-analytics-api-openapi.yml
  - openapi/contentstack-automate-management-api-openapi.yml
  - openapi/contentstack-brand-kit-management-api-openapi.yml
  - openapi/contentstack-generative-ai-api-openapi.yml
  - openapi/contentstack-knowledge-vault-api-openapi.yml
  - openapi/contentstack-launch-api-openapi.yml
  - openapi/contentstack-personalize-management-api-openapi.yml
  - openapi/contentstack-scim-api-openapi.yml
  type: http
- description: Contentstack user authtoken. Only organization Owners and Admins can access analytics.
  in: header
  name: authtokenAuth
  parameter: authtoken
  sources:
  - openapi/contentstack-analytics-api-openapi.yml
  - openapi/contentstack-automate-management-api-openapi.yml
  - openapi/contentstack-brand-kit-management-api-openapi.yml
  - openapi/contentstack-content-management-api-openapi.yml
  - openapi/contentstack-generative-ai-api-openapi.yml
  - openapi/contentstack-knowledge-vault-api-openapi.yml
  - openapi/contentstack-launch-api-openapi.yml
  - openapi/contentstack-personalize-management-api-openapi.yml
  type: apiKey
- description: The API key for the Contentstack stack.
  in: header
  name: apiKey
  parameter: api_key
  sources:
  - openapi/contentstack-content-delivery-api-openapi.yml
  type: apiKey
- description: The delivery token granting read access to the stack environment.
  in: header
  name: deliveryToken
  parameter: access_token
  sources:
  - openapi/contentstack-content-delivery-api-openapi.yml
  type: apiKey
- description: Management token in the format "Bearer {management_token}" for server-to-server authentication without user sessions.
  in: header
  name: managementTokenAuth
  parameter: authorization
  sources:
  - openapi/contentstack-content-management-api-openapi.yml
  type: apiKey
slug: contentstack-authentication
source_filename: contentstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/contentstack-analytics-api-openapi.yml, openapi/contentstack-automate-management-api-openapi.yml,\n  openapi/contentstack-brand-kit-management-api-openapi.yml, openapi/contentstack-content-delivery-api-openapi.yml,\n  openapi/contentstack-content-management-api-openapi.yml, openapi/contentstack-generative-ai-api-openapi.yml,\n  openapi/contentstack-knowledge-vault-api-openapi.yml, openapi/contentstack-launch-api-openapi.yml,\n  openapi/contentstack-personalize-management-api-openapi.yml, openapi/contentstack-scim-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token (M2M) with analytics access.\n  sources:\n  - openapi/contentstack-analytics-api-openapi.yml\n  - openapi/contentstack-automate-management-api-openapi.yml\n  - openapi/contentstack-brand-kit-management-api-openapi.yml\n  - openapi/contentstack-generative-ai-api-openapi.yml\n\
  \  - openapi/contentstack-knowledge-vault-api-openapi.yml\n  - openapi/contentstack-launch-api-openapi.yml\n  - openapi/contentstack-personalize-management-api-openapi.yml\n  - openapi/contentstack-scim-api-openapi.yml\n- name: authtokenAuth\n  type: apiKey\n  in: header\n  parameter: authtoken\n  description: Contentstack user authtoken. Only organization Owners and Admins can access analytics.\n  sources:\n  - openapi/contentstack-analytics-api-openapi.yml\n  - openapi/contentstack-automate-management-api-openapi.yml\n  - openapi/contentstack-brand-kit-management-api-openapi.yml\n  - openapi/contentstack-content-management-api-openapi.yml\n  - openapi/contentstack-generative-ai-api-openapi.yml\n  - openapi/contentstack-knowledge-vault-api-openapi.yml\n  - openapi/contentstack-launch-api-openapi.yml\n  - openapi/contentstack-personalize-management-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: The API key for the Contentstack stack.\n\
  \  sources:\n  - openapi/contentstack-content-delivery-api-openapi.yml\n- name: deliveryToken\n  type: apiKey\n  in: header\n  parameter: access_token\n  description: The delivery token granting read access to the stack environment.\n  sources:\n  - openapi/contentstack-content-delivery-api-openapi.yml\n- name: managementTokenAuth\n  type: apiKey\n  in: header\n  parameter: authorization\n  description: Management token in the format \"Bearer {management_token}\" for server-to-server\n    authentication without user sessions.\n  sources:\n  - openapi/contentstack-content-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/contentstack/refs/heads/main/authentication/contentstack-authentication.yml
summary_line: apiKey/http · 5 schemes
tags: []
---
