---
anonymous_access: false
api_key_in: []
api_specs:
- filename: creatorriver-com-account-api-openapi.yml
  format: yaml
  label: Creator River Account API
  slug: creatorriver-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatorriver-com/openapi/creatorriver-com-account-api-openapi.yml
- filename: creatorriver-com-campaigns-api-openapi.yml
  format: yaml
  label: Creator River Campaigns API
  slug: creatorriver-com-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatorriver-com/openapi/creatorriver-com-campaigns-api-openapi.yml
- filename: creatorriver-com-contacts-api-openapi.yml
  format: yaml
  label: Creator River Contacts API
  slug: creatorriver-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatorriver-com/openapi/creatorriver-com-contacts-api-openapi.yml
- filename: creatorriver-com-conversations-api-openapi.yml
  format: yaml
  label: Creator River Conversations API
  slug: creatorriver-com-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatorriver-com/openapi/creatorriver-com-conversations-api-openapi.yml
- filename: creatorriver-com-creators-api-openapi.yml
  format: yaml
  label: Creator River Creators API
  slug: creatorriver-com-creators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatorriver-com/openapi/creatorriver-com-creators-api-openapi.yml
- filename: creatorriver-com-emails-api-openapi.yml
  format: yaml
  label: Creator River Emails API
  slug: creatorriver-com-emails-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatorriver-com/openapi/creatorriver-com-emails-api-openapi.yml
- filename: creatorriver-com-searches-api-openapi.yml
  format: yaml
  label: Creator River Searches API
  slug: creatorriver-com-searches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatorriver-com/openapi/creatorriver-com-searches-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Creator River Authentication
name_suffix: Authentication
oauth_flows: []
overview: Creator River secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Creator River
provider_slug: creatorriver-com
scheme_count: 1
schemes:
- description: An API key from https://www.creatorriver.com/settings/apikeys
  name: apiKey
  scheme: bearer
  sources:
  - openapi/creatorriver-com-openapi.yml
  type: http
slug: creatorriver-com-authentication
source_filename: creatorriver-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.creatorriver.com/mcp\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: An API key from https://www.creatorriver.com/settings/apikeys\n  sources:\n  - openapi/creatorriver-com-openapi.yml\ndocs: https://www.creatorriver.com/mcp\nnotes:\n- Claude, ChatGPT and other custom-connector apps sign in to Creator River and approve\n  the app (no key needed) on the MCP endpoint.\n- 'Claude Code, Cursor and other MCP clients and the REST API send \"Authorization:\n  Bearer YOUR_API_KEY\"; keys are created in Settings → API keys (https://www.creatorriver.com/settings/apikeys).'\n- The creatorriver CLI obtains a key via browser approval (creatorriver auth login)\n  or CREATORRIVER_API_KEY.\n"
source_yaml_url: https://artifacts.apis.io/creatorriver-com/authentication/creatorriver-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Influencer Marketing
- Creator Search
- Influencer Outreach
- Email Finder
- YouTube
- TikTok
- Instagram
- MCP
- AI Agents
---
