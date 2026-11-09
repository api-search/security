---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: creavily-admin-api-openapi.yml
  format: yaml
  label: Creavily Admin API
  slug: creavily-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-admin-api-openapi.yml
- filename: creavily-agent-api-openapi.yml
  format: yaml
  label: Creavily Agent API
  slug: creavily-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-agent-api-openapi.yml
- filename: creavily-analytics-api-openapi.yml
  format: yaml
  label: Creavily Analytics API
  slug: creavily-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-analytics-api-openapi.yml
- filename: creavily-assets-api-openapi.yml
  format: yaml
  label: Creavily Assets API
  slug: creavily-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-assets-api-openapi.yml
- filename: creavily-auth-api-openapi.yml
  format: yaml
  label: Creavily Auth API
  slug: creavily-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-auth-api-openapi.yml
- filename: creavily-automations-api-openapi.yml
  format: yaml
  label: Creavily Automations API
  slug: creavily-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-automations-api-openapi.yml
- filename: creavily-billing-api-openapi.yml
  format: yaml
  label: Creavily Billing API
  slug: creavily-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-billing-api-openapi.yml
- filename: creavily-blog-api-openapi.yml
  format: yaml
  label: Creavily Blog API
  slug: creavily-blog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-blog-api-openapi.yml
- filename: creavily-brands-api-openapi.yml
  format: yaml
  label: Creavily Brands API
  slug: creavily-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-brands-api-openapi.yml
- filename: creavily-bridges-api-openapi.yml
  format: yaml
  label: Creavily Bridges API
  slug: creavily-bridges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-bridges-api-openapi.yml
- filename: creavily-channels-api-openapi.yml
  format: yaml
  label: Creavily Channels API
  slug: creavily-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-channels-api-openapi.yml
- filename: creavily-developer-api-openapi.yml
  format: yaml
  label: Creavily Developer API
  slug: creavily-developer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-developer-api-openapi.yml
- filename: creavily-engagement-api-openapi.yml
  format: yaml
  label: Creavily Engagement API
  slug: creavily-engagement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-engagement-api-openapi.yml
- filename: creavily-inquiries-api-openapi.yml
  format: yaml
  label: Creavily Inquiries API
  slug: creavily-inquiries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-inquiries-api-openapi.yml
- filename: creavily-media-api-openapi.yml
  format: yaml
  label: Creavily Media API
  slug: creavily-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-media-api-openapi.yml
- filename: creavily-oauth-api-openapi.yml
  format: yaml
  label: Creavily OAuth API
  slug: creavily-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-oauth-api-openapi.yml
- filename: creavily-platform-api-openapi.yml
  format: yaml
  label: Creavily Platform API
  slug: creavily-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-platform-api-openapi.yml
- filename: creavily-provider-tools-api-openapi.yml
  format: yaml
  label: Creavily Provider Tools API
  slug: creavily-provider-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-provider-tools-api-openapi.yml
- filename: creavily-publishing-api-openapi.yml
  format: yaml
  label: Creavily Publishing API
  slug: creavily-publishing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-publishing-api-openapi.yml
- filename: creavily-system-api-openapi.yml
  format: yaml
  label: Creavily System API
  slug: creavily-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-system-api-openapi.yml
- filename: creavily-webhooks-api-openapi.yml
  format: yaml
  label: Creavily Webhooks API
  slug: creavily-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creavily/openapi/creavily-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: derived
name: Creavily Authentication
name_suffix: Authentication
oauth_flows: []
overview: Creavily secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Creavily
provider_slug: creavily
scheme_count: 5
schemes:
- description: Use a Creavily API key or OAuth access token. Public endpoints are scoped to the authenticated principal organization.
  name: publicBearer
  scheme: bearer
  sources:
  - openapi/creavily-openapi.json
  type: http
- description: Host-only HttpOnly Dashboard session cookie issued after the one-time browser-session exchange. Browser clients rely on credentialed requests and an approved Origin; JavaScript does not read this value.
  in: cookie
  name: dashboardSessionCookie
  parameter: creavily_dashboard_session
  sources:
  - openapi/creavily-openapi.json
  type: apiKey
- description: Internal service credential for non-public operational routes. It is never exposed to browser or third-party clients.
  in: header
  name: internalServiceToken
  parameter: x-creavily-internal-token
  sources:
  - openapi/creavily-openapi.json
  type: apiKey
- description: Server-side service-principal credential accepted by policy-gated admin routes. It is never exposed to browser or third-party clients.
  in: header
  name: servicePrincipalToken
  parameter: x-creavily-service-principal-token
  sources:
  - openapi/creavily-openapi.json
  type: apiKey
- description: Short-lived HttpOnly temporary cookie used only with POST /v1/auth/browser-session/exchange. It is cleared after a successful exchange or logout.
  in: cookie
  name: browserSessionExchangeCookie
  parameter: creavily_browser_session_exchange
  sources:
  - openapi/creavily-openapi.json
  type: apiKey
slug: creavily-authentication
source_filename: creavily-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/creavily-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: publicBearer\n  type: http\n  scheme: bearer\n  description: Use a Creavily API key or OAuth access token. Public endpoints are scoped to\n    the authenticated principal organization.\n  sources:\n  - openapi/creavily-openapi.json\n- name: dashboardSessionCookie\n  type: apiKey\n  in: cookie\n  parameter: creavily_dashboard_session\n  description: Host-only HttpOnly Dashboard session cookie issued after the one-time browser-session\n    exchange. Browser clients rely on credentialed requests and an approved Origin; JavaScript\n    does not read this value.\n  sources:\n  - openapi/creavily-openapi.json\n- name: internalServiceToken\n  type: apiKey\n  in: header\n  parameter: x-creavily-internal-token\n  description: Internal service credential for non-public operational routes. It is never exposed\n\
  \    to browser or third-party clients.\n  sources:\n  - openapi/creavily-openapi.json\n- name: servicePrincipalToken\n  type: apiKey\n  in: header\n  parameter: x-creavily-service-principal-token\n  description: Server-side service-principal credential accepted by policy-gated admin routes.\n    It is never exposed to browser or third-party clients.\n  sources:\n  - openapi/creavily-openapi.json\n- name: browserSessionExchangeCookie\n  type: apiKey\n  in: cookie\n  parameter: creavily_browser_session_exchange\n  description: Short-lived HttpOnly temporary cookie used only with POST /v1/auth/browser-session/exchange.\n    It is cleared after a successful exchange or logout.\n  sources:\n  - openapi/creavily-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/creavily/authentication/creavily-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Social Media
- E-Commerce
- Publishing
- Automation
---
