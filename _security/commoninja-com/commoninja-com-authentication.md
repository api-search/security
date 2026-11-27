---
anonymous_access: false
api_key_in: []
api_specs:
- filename: commoninja-com-openapi-generated.yml
  format: yaml
  label: Common Ninja Platform API
  slug: commoninja-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commoninja-com/openapi/_ae-authored/commoninja-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Common Ninja Authentication
name_suffix: Authentication
oauth_flows: []
overview: Common Ninja declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Common Ninja
provider_slug: commoninja-com
scheme_count: 5
schemes:
- applies_to: Platform API (https://api.commoninja.com/platform/api/v1) - app level access
  authorizationUrl: https://api.commoninja.com/oauth/authorize
  flow: authorizationCode
  name: oauth2
  note: Docs list the token endpoint as "GET /oauth/token" while their examples POST form-encoded; supports authorization_code and refresh_token grants. The scope parameter is commented out in the docs.
  refresh: true
  tokenUrl: https://api.commoninja.com/oauth/token
  type: oauth2
  usage: 'Authorization: Bearer ACCESS_TOKEN'
- applies_to: Platform API - account level access (own account resources); also accepted by the hosted MCP server
  header: CN-API-Token
  in: header
  name: CN-API-Token
  type: apiKey
- applies_to: Platform API - reseller / white label partners; tenant ID scopes requests per end-user or site
  companion_header: CN-Reseller-Tenant-ID
  header: CN-Reseller-Token
  in: header
  name: reseller
  type: apiKey
- applies_to: Developer Apps (Integrations) API (https://api.commoninja.com/integrations/api/v1)
  name: app-basic
  scheme: basic
  type: http
  value: Basic base64(appId:appSecret)
- applies_to: Integrations API - merchant token obtained via https://integrations.commoninja.com/integrations/{PLATFORM_NAME}/{CN_APP_ID}/oauth/authenticate, sent together with the Basic app header
  header: X-CN-User-Access-Token
  in: header
  name: X-CN-User-Access-Token
  type: apiKey
slug: commoninja-com-authentication
source_filename: commoninja-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://developers.commoninja.com/docs/authentication/overview\n- https://developers.commoninja.com/docs/authentication/authorization\n- https://developers.commoninja.com/docs/authentication/tokens\n- https://developers.commoninja.com/docs/authentication/requests\n- https://developers.commoninja.com/docs/white-label/authentication\n- https://docs.commoninja.com/getting-started/api-authorization.md\n- https://docs.commoninja.com/getting-started/authentication/using-the-access-token.md\ndocs: https://developers.commoninja.com/docs/authentication/overview\nschemes:\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://api.commoninja.com/oauth/authorize\n  tokenUrl: https://api.commoninja.com/oauth/token\n  refresh: true\n  usage: 'Authorization: Bearer ACCESS_TOKEN'\n  applies_to: Platform API (https://api.commoninja.com/platform/api/v1) - app level access\n  note: Docs list the token endpoint\
  \ as \"GET /oauth/token\" while their examples POST form-encoded; supports authorization_code and refresh_token grants. The scope parameter is commented out in the docs.\n- name: CN-API-Token\n  type: apiKey\n  in: header\n  header: CN-API-Token\n  applies_to: Platform API - account level access (own account resources); also accepted by the hosted MCP server\n- name: reseller\n  type: apiKey\n  in: header\n  header: CN-Reseller-Token\n  companion_header: CN-Reseller-Tenant-ID\n  applies_to: Platform API - reseller / white label partners; tenant ID scopes requests per end-user or site\n- name: app-basic\n  type: http\n  scheme: basic\n  value: Basic base64(appId:appSecret)\n  applies_to: Developer Apps (Integrations) API (https://api.commoninja.com/integrations/api/v1)\n- name: X-CN-User-Access-Token\n  type: apiKey\n  in: header\n  header: X-CN-User-Access-Token\n  applies_to: Integrations API - merchant token obtained via https://integrations.commoninja.com/integrations/{PLATFORM_NAME}/{CN_APP_ID}/oauth/authenticate,\
  \ sent together with the Basic app header\nwebhook_signing:\n  header: X-CN-Webhook-Signature\n  algorithm: HMAC-SHA256 of the JSON body with the appSecret, base64\n  source: https://docs.commoninja.com/getting-started/webhooks/verifying-webhooks.md\n"
source_yaml_url: https://artifacts.apis.io/commoninja-com/authentication/commoninja-com-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Widgets
- No-Code
- Website Builder
- White Label
- Webhook
- E-Commerce
- Developer Platform
---
