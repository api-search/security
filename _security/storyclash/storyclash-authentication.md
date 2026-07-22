---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Storyclash Authentication
name_suffix: Authentication
oauth_flows: []
overview: Storyclash secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Storyclash
provider_slug: storyclash
scheme_count: 1
schemes:
- description: Token-based authentication. Storyclash provisions an API token per customer that is sent on each request. Rate limiting is configurable per token/campaign (default 1 request/hour per campaign, adjustable for enterprise).
  in: header
  name: apiToken
  sources:
  - https://www.storyclash.com/integrations/api-integration
  type: apiKey
slug: storyclash-authentication
source_filename: storyclash-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.storyclash.com/integrations/api-integration\ndocs: https://storyclash.notion.site/Storyclash-API-Documentation-1266dc2ddd0880a79cf9e3d34c19fa01\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Storyclash publishes no machine-readable OpenAPI. The API integration page and\n    the Notion API documentation describe a single token-based authentication model\n    over HTTPS. No OAuth2 or OpenID Connect surface is documented, so scopes/ is not\n    applicable.\nschemes:\n- name: apiToken\n  type: apiKey\n  in: header\n  description: >-\n    Token-based authentication. Storyclash provisions an API token per customer\n    that is sent on each request. Rate limiting is configurable per token/campaign\n    (default 1 request/hour per campaign, adjustable for enterprise).\n  sources: [https://www.storyclash.com/integrations/api-integration]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storyclash/refs/heads/main/authentication/storyclash-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Influencer Marketing
- Creator Economy
- Social Media Analytics
- Marketing Analytics
- Campaign Management
- Business Intelligence
- REST API
- Webhooks
---
