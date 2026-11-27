---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cleo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cleo declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cleo
provider_slug: cleofamily-app
scheme_count: 2
schemes:
- applies_to: https://api.cleofamily.app/mcp
  evidence: You sign in on Cleo's own login page using OAuth 2.1 with PKCE, so your assistant never sees your password.
  flow: authorizationCode
  name: cleo-oauth
  note: Authorization and token endpoint URLs are not published in the docs and were not called.
  pkce: true
  standard: OAuth 2.1
  type: oauth2
- applies_to: cleo-cli
  evidence: 'Headless: set CLEO_REFRESH_TOKEN to the refresh_token from ~/.cleo/credentials.json on a machine that ran cleo login. (CLEO_ACCESS_TOKEN also works, for an hour.)'
  name: cleo-cli-token
  note: Bearer transport is inferred from the access/refresh-token wording in the README; the header is not stated.
  scheme: bearer
  source: https://registry.npmjs.org/cleo-cli
  type: http
slug: cleofamily-app-authentication
source_filename: cleofamily-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://www.cleofamily.app/assistant/docs\ndocs: https://www.cleofamily.app/assistant/docs\nsummary: The Cleo connector (remote MCP, Streamable HTTP, https://api.cleofamily.app/mcp) authenticates with OAuth 2.1 and PKCE on Cleo's own login page. Access is granted area by area (see, see and change, or off) at connect time and can be revoked from the assistant's connector settings. No OpenAPI or published scope names exist. The unauthenticated endpoint answered HTTP 401 in pre-flight (2026-11-04).\nschemes:\n- name: cleo-oauth\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  standard: OAuth 2.1\n  applies_to: https://api.cleofamily.app/mcp\n  evidence: \"You sign in on Cleo's own login page using OAuth 2.1 with PKCE, so your assistant never sees your password.\"\n  note: Authorization and token endpoint URLs are not published in the docs and were not called.\n- name: cleo-cli-token\n  type: http\n  scheme: bearer\n\
  \  applies_to: cleo-cli\n  evidence: 'Headless: set CLEO_REFRESH_TOKEN to the refresh_token from ~/.cleo/credentials.json on a machine that ran cleo login. (CLEO_ACCESS_TOKEN also works, for an hour.)'\n  source: https://registry.npmjs.org/cleo-cli\n  note: Bearer transport is inferred from the access/refresh-token wording in the README; the header is not stated.\n"
source_yaml_url: https://artifacts.apis.io/cleofamily-app/authentication/cleofamily-app-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Family
- Parenting
- Baby Tracking
- Meal Planning
- MCP
- AI Assistant
- Productivity
---
