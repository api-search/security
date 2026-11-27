---
anonymous_access: false
api_key_in: []
api_specs:
- filename: outreachgenie-ai-content-api-openapi.yml
  format: yaml
  label: OutreachGenie Content API
  slug: outreachgenie-ai-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outreachgenie-ai/openapi/outreachgenie-ai-content-api-openapi.yml
- filename: outreachgenie-ai-integration-api-openapi.yml
  format: yaml
  label: OutreachGenie Integration API
  slug: outreachgenie-ai-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outreachgenie-ai/openapi/outreachgenie-ai-integration-api-openapi.yml
- filename: outreachgenie-ai-profile-tracker-api-openapi.yml
  format: yaml
  label: OutreachGenie Profile Tracker API
  slug: outreachgenie-ai-profile-tracker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outreachgenie-ai/openapi/outreachgenie-ai-profile-tracker-api-openapi.yml
- filename: outreachgenie-ai-runtime-api-openapi.yml
  format: yaml
  label: OutreachGenie Runtime API
  slug: outreachgenie-ai-runtime-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outreachgenie-ai/openapi/outreachgenie-ai-runtime-api-openapi.yml
- filename: outreachgenie-ai-writing-api-openapi.yml
  format: yaml
  label: OutreachGenie Writing API
  slug: outreachgenie-ai-writing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/outreachgenie-ai/openapi/outreachgenie-ai-writing-api-openapi.yml
auth_types: []
description: Authentication methods for OutreachGenie MCP APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: OutreachGenie Authentication
name_suffix: Authentication
oauth_flows: []
overview: OutreachGenie declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: OutreachGenie
provider_slug: outreachgenie-ai
scheme_count: 2
schemes:
- evidence: 'Copy curl -H "Authorization: Bearer $LINKEDIN_CRM_API_KEY" "$LINKEDIN_CRM_API_BASE_URL/api/v1/runtime/auth/verify"'
  header: Authorization
  how_to_obtain: Create an OutreachGenie API key in Settings → API keys and set it in the environment variable LINKEDIN_CRM_API_KEY.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'OAuth connections ChatGPT and Claude connect through OutreachGenie''s OAuth flow: sign in, choose a workspace, and approve only the requested scopes.'
  how_to_obtain: Sign in, choose a workspace, and approve the requested scopes during the OAuth consent flow.
  name: OutreachGenie OAuth flow
  type: oauth2
slug: outreachgenie-ai-authentication
source_filename: outreachgenie-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.outreachgenie.ai/linkedin-boolean-search-builder
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.outreachgenie.ai/linkedin-boolean-search-builder\nsources:\n- https://www.outreachgenie.ai/linkedin-boolean-search-builder\n- https://www.outreachgenie.ai/blog/create-linkedin-company-page\n- https://app.outreachgenie.ai/docs/mcp/codex\n- https://app.outreachgenie.ai/docs/mcp/claude\ndescription: Authentication methods for OutreachGenie MCP APIs\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Copy curl -H \"Authorization: Bearer $LINKEDIN_CRM_API_KEY\" \"$LINKEDIN_CRM_API_BASE_URL/api/v1/runtime/auth/verify\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an OutreachGenie API key in Settings → API keys and set it in the environment variable LINKEDIN_CRM_API_KEY.\n- type: oauth2\n  name: OutreachGenie OAuth flow\n  evidence: 'OAuth connections ChatGPT and Claude connect through OutreachGenie''s OAuth flow: sign in, choose a workspace,\
  \ and approve only the\n    requested scopes.'\n  how_to_obtain: Sign in, choose a workspace, and approve the requested scopes during the OAuth consent flow.\ndocs: https://www.outreachgenie.ai/linkedin-boolean-search-builder\n"
source_yaml_url: https://artifacts.apis.io/outreachgenie-ai/authentication/outreachgenie-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Automation
- LinkedIn
- Outreach
- Artificial Intelligence
---
