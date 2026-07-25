---
api_key_in:
- header
api_specs:
- filename: adobe-campaign-custom-resources-api-openapi.yml
  format: yaml
  label: Adobe Campaign Custom Resources API
  slug: adobe-campaign-custom-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-custom-resources-api-openapi.yml
- filename: adobe-campaign-data-management-api-openapi.yml
  format: yaml
  label: Adobe Campaign Data Management API
  slug: adobe-campaign-data-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-data-management-api-openapi.yml
- filename: adobe-campaign-delivery-api-openapi.yml
  format: yaml
  label: Adobe Campaign Delivery API
  slug: adobe-campaign-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-delivery-api-openapi.yml
- filename: adobe-campaign-marketing-history-api-openapi.yml
  format: yaml
  label: Adobe Campaign Marketing History API
  slug: adobe-campaign-marketing-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-marketing-history-api-openapi.yml
- filename: adobe-campaign-metadata-api-openapi.yml
  format: yaml
  label: Adobe Campaign Metadata API
  slug: adobe-campaign-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-metadata-api-openapi.yml
- filename: adobe-campaign-organizational-units-api-openapi.yml
  format: yaml
  label: Adobe Campaign Organizational Units API
  slug: adobe-campaign-organizational-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-organizational-units-api-openapi.yml
- filename: adobe-campaign-privacy-api-openapi.yml
  format: yaml
  label: Adobe Campaign Privacy API
  slug: adobe-campaign-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-privacy-api-openapi.yml
- filename: adobe-campaign-profileandservices-api-openapi.yml
  format: yaml
  label: Adobe Campaign ProfileAndServices API
  slug: adobe-campaign-profileandservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-profileandservices-api-openapi.yml
- filename: adobe-campaign-profiles-api-openapi.yml
  format: yaml
  label: Adobe Campaign Profiles API
  slug: adobe-campaign-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-profiles-api-openapi.yml
- filename: adobe-campaign-query-definition-api-openapi.yml
  format: yaml
  label: Adobe Campaign Query Definition API
  slug: adobe-campaign-query-definition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-query-definition-api-openapi.yml
- filename: adobe-campaign-real-time-events-api-openapi.yml
  format: yaml
  label: Adobe Campaign Real-Time Events API
  slug: adobe-campaign-real-time-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-real-time-events-api-openapi.yml
- filename: adobe-campaign-session-management-api-openapi.yml
  format: yaml
  label: Adobe Campaign Session Management API
  slug: adobe-campaign-session-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-session-management-api-openapi.yml
- filename: adobe-campaign-subscription-api-openapi.yml
  format: yaml
  label: Adobe Campaign Subscription API
  slug: adobe-campaign-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-subscription-api-openapi.yml
- filename: adobe-campaign-subscriptions-api-openapi.yml
  format: yaml
  label: Adobe Campaign Subscriptions API
  slug: adobe-campaign-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-subscriptions-api-openapi.yml
- filename: adobe-campaign-transactional-messages-api-openapi.yml
  format: yaml
  label: Adobe Campaign Transactional Messages API
  slug: adobe-campaign-transactional-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-transactional-messages-api-openapi.yml
- filename: adobe-campaign-workflow-api-openapi.yml
  format: yaml
  label: Adobe Campaign Workflow API
  slug: adobe-campaign-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-workflow-api-openapi.yml
- filename: adobe-campaign-workflows-api-openapi.yml
  format: yaml
  label: Adobe Campaign Workflows API
  slug: adobe-campaign-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/openapi/adobe-campaign-workflows-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Adobe Campaign Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adobe Campaign secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Adobe Campaign
provider_slug: adobe-campaign
scheme_count: 3
schemes:
- description: Security token obtained from xtk:session#Logon. Must be passed alongside the session token cookie (__sessiontoken) on all authenticated requests. Tokens have a 24-hour lifecycle.
  in: header
  name: SessionToken
  parameter: X-Security-Token
  sources:
  - openapi/adobe-campaign-classic-openapi-original.yml
  type: apiKey
- bearerFormat: JWT
  description: OAuth Server-to-Server access token obtained from Adobe IMS at https://ims-na1.adobelogin.com/ims/token/v3
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/adobe-campaign-standard-openapi-original.yml
  type: http
- description: Your Adobe Developer Console API Key (Client ID).
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/adobe-campaign-standard-openapi-original.yml
  type: apiKey
slug: adobe-campaign-authentication
source_filename: adobe-campaign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/adobe-campaign-classic-openapi-original.yml, openapi/adobe-campaign-standard-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: SessionToken\n  type: apiKey\n  in: header\n  parameter: X-Security-Token\n  description: Security token obtained from xtk:session#Logon. Must be passed alongside the\n    session token cookie (__sessiontoken) on all authenticated requests. Tokens have a 24-hour\n    lifecycle.\n  sources:\n  - openapi/adobe-campaign-classic-openapi-original.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth Server-to-Server access token obtained from Adobe IMS at https://ims-na1.adobelogin.com/ims/token/v3\n  sources:\n  - openapi/adobe-campaign-standard-openapi-original.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Your Adobe Developer Console API Key (Client\
  \ ID).\n  sources:\n  - openapi/adobe-campaign-standard-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/authentication/adobe-campaign-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
---
