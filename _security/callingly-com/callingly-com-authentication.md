---
anonymous_access: false
api_key_in: []
api_specs:
- filename: callingly-com-openapi-generated.yml
  format: yaml
  label: Callingly API
  slug: callingly-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callingly-com/openapi/_ae-authored/callingly-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Callingly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Callingly declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Callingly
provider_slug: callingly-com
scheme_count: 2
schemes:
- description: 'The API requires generating a Bearer Token to be used with every request. Keys are created under Settings -> API Keys in the dashboard; the key cannot be viewed again after creation. Every request also sends Accept: application/json.'
  format: 'Authorization : Bearer {{YOUR_BEARER_TOKEN_HERE}}'
  header: Authorization
  in: header
  key_management: dashboard (Settings -> API Keys); revocable from the dashboard
  name: bearerToken
  scheme: bearer
  type: http
- applies_to: https://api.callingly.com/mcp
  description: 'The MCP page (https://callingly.com/features/mcp) instructs pasting a dashboard API key as the bearer token ("Authorization": "Bearer clly_live_..."). The github.com/callingly/mcp repo description calls the hosted server "(OAuth)"; no OAuth flow, authorization server or scope list is documented.'
  name: mcpBearer
  scheme: bearer
  type: http
slug: callingly-com-authentication
source_filename: callingly-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://help.callingly.com/article/38-callingly-api-documentation\ndocs: https://help.callingly.com/article/38-callingly-api-documentation\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization : Bearer {{YOUR_BEARER_TOKEN_HERE}}'\n  description: 'The API requires generating a Bearer Token to be used with every request. Keys are created under Settings -> API Keys in the dashboard; the key cannot be viewed again after creation. Every request also sends Accept: application/json.'\n  key_management: dashboard (Settings -> API Keys); revocable from the dashboard\n- name: mcpBearer\n  type: http\n  scheme: bearer\n  applies_to: https://api.callingly.com/mcp\n  description: 'The MCP page (https://callingly.com/features/mcp) instructs pasting a dashboard API key as the bearer token (\"Authorization\": \"Bearer clly_live_...\"). The github.com/callingly/mcp repo\
  \ description calls the hosted server \"(OAuth)\"; no OAuth flow, authorization server or scope list is documented.'\nmulti_tenancy: If you are an Agency partner and are using the API to make requests for your clients, along with your Bearer Token you can pass in an account_id parameter with the ID number of your client's account.\nrole_requirements:\n- Managing routing requires an owner or admin API key.\n- Managing sequences requires an owner, admin or manager API key.\n"
source_yaml_url: https://artifacts.apis.io/callingly-com/authentication/callingly-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Sales
- Lead Response
- Speed To Lead
- Telephony
- SMS
- AI Voice Agents
- MCP
---
