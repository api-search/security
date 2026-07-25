---
api_key_in:
- header
api_specs:
- filename: dixa-agents-api-openapi.yml
  format: yaml
  label: Dixa Agents API
  slug: dixa-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-agents-api-openapi.yml
- filename: dixa-analytics-api-openapi.yml
  format: yaml
  label: Dixa Analytics API
  slug: dixa-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-analytics-api-openapi.yml
- filename: dixa-anonymization-api-openapi.yml
  format: yaml
  label: Dixa Anonymization API
  slug: dixa-anonymization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-anonymization-api-openapi.yml
- filename: dixa-business-hours-api-openapi.yml
  format: yaml
  label: Dixa Business Hours API
  slug: dixa-business-hours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-business-hours-api-openapi.yml
- filename: dixa-chatbots-api-openapi.yml
  format: yaml
  label: Dixa Chatbots API
  slug: dixa-chatbots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-chatbots-api-openapi.yml
- filename: dixa-contact-endpoints-api-openapi.yml
  format: yaml
  label: Dixa Contact Endpoints API
  slug: dixa-contact-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-contact-endpoints-api-openapi.yml
- filename: dixa-conversations-api-openapi.yml
  format: yaml
  label: Dixa Conversations API
  slug: dixa-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-conversations-api-openapi.yml
- filename: dixa-custom-attributes-api-openapi.yml
  format: yaml
  label: Dixa Custom Attributes API
  slug: dixa-custom-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-custom-attributes-api-openapi.yml
- filename: dixa-end-users-api-openapi.yml
  format: yaml
  label: Dixa End Users API
  slug: dixa-end-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-end-users-api-openapi.yml
- filename: dixa-internal-notes-api-openapi.yml
  format: yaml
  label: Dixa Internal Notes API
  slug: dixa-internal-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-internal-notes-api-openapi.yml
- filename: dixa-knowledge-api-openapi.yml
  format: yaml
  label: Dixa Knowledge API
  slug: dixa-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-knowledge-api-openapi.yml
- filename: dixa-messages-api-openapi.yml
  format: yaml
  label: Dixa Messages API
  slug: dixa-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-messages-api-openapi.yml
- filename: dixa-organization-api-openapi.yml
  format: yaml
  label: Dixa Organization API
  slug: dixa-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-organization-api-openapi.yml
- filename: dixa-queues-api-openapi.yml
  format: yaml
  label: Dixa Queues API
  slug: dixa-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-queues-api-openapi.yml
- filename: dixa-ratings-api-openapi.yml
  format: yaml
  label: Dixa Ratings API
  slug: dixa-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-ratings-api-openapi.yml
- filename: dixa-search-api-openapi.yml
  format: yaml
  label: Dixa Search API
  slug: dixa-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-search-api-openapi.yml
- filename: dixa-tags-api-openapi.yml
  format: yaml
  label: Dixa Tags API
  slug: dixa-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-tags-api-openapi.yml
- filename: dixa-teams-api-openapi.yml
  format: yaml
  label: Dixa Teams API
  slug: dixa-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-teams-api-openapi.yml
- filename: dixa-templates-api-openapi.yml
  format: yaml
  label: Dixa Templates API
  slug: dixa-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-templates-api-openapi.yml
- filename: dixa-webhooks-api-openapi.yml
  format: yaml
  label: Dixa Webhooks API
  slug: dixa-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/openapi/dixa-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dixa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dixa secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dixa
provider_slug: dixa
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/dixa-api.yaml
  type: apiKey
slug: dixa-authentication
source_filename: dixa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dixa-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/dixa-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dixa/refs/heads/main/authentication/dixa-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Customer Service
- Conversational
- Omnichannel
- CX
- Help Desk
- Chat
- Knowledge Base
---
