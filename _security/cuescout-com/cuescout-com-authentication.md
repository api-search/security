---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CueScout Authentication
name_suffix: Authentication
oauth_flows: []
overview: CueScout declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CueScout
provider_slug: cuescout-com
scheme_count: 3
schemes:
- applies_to:
  - check_ai_visibility
  - check_ai_readiness
  - check_ai_crawler_access
  - validate_structured_data
  - check_sitemap
  evidence: There is no API key and nothing to install.
  name: none (public MCP checks)
  type: none
- applies_to:
  - get_ai_visibility
  - list_prompts
  - get_prompt_answers
  - list_citation_sources
  - list_todos
  - get_todo
  - get_site_audit
  - list_brands
  - get_profile
  authorization_server: https://api.cuescout.com
  evidence: You sign in on cuescout.com, approve it once, and from then on the chat can read what CueScout has already collected for you.
  name: OAuth account connection
  note: Docs state "Signing in to your CueScout account works in ChatGPT for now." Authorization server and scope are as recorded in apis.yml from the live MCP probe; endpoints were not called.
  scopes:
  - account:read
  type: oauth2
- evidence: 'Every request carries an X-CueScout-Signature header: an HMAC-SHA256 of the exact body, under a secret shown on the settings screen.'
  header: X-CueScout-Signature
  name: webhook signature (outbound)
  source: https://cuescout.com/integrations/zapier
  type: hmac
slug: cuescout-com-authentication
source_filename: cuescout-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cuescout.com/mcp\ndocs: https://cuescout.com/mcp\nname: CueScout authentication\nschemes:\n- name: none (public MCP checks)\n  type: none\n  applies_to: [check_ai_visibility, check_ai_readiness, check_ai_crawler_access, validate_structured_data, check_sitemap]\n  evidence: 'There is no API key and nothing to install.'\n- name: OAuth account connection\n  type: oauth2\n  authorization_server: https://api.cuescout.com\n  scopes: [account:read]\n  applies_to: [get_ai_visibility, list_prompts, get_prompt_answers, list_citation_sources, list_todos, get_todo, get_site_audit, list_brands, get_profile]\n  evidence: 'You sign in on cuescout.com, approve it once, and from then on the chat can read what CueScout has already collected for you.'\n  note: Docs state \"Signing in to your CueScout account works in ChatGPT for now.\" Authorization server and scope are as recorded in apis.yml from the live MCP probe; endpoints were not\
  \ called.\n- name: webhook signature (outbound)\n  type: hmac\n  header: X-CueScout-Signature\n  evidence: 'Every request carries an X-CueScout-Signature header: an HMAC-SHA256 of the exact body, under a secret shown on the settings screen.'\n  source: https://cuescout.com/integrations/zapier\n"
source_yaml_url: https://artifacts.apis.io/cuescout-com/authentication/cuescout-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- AI Visibility
- Generative Engine Optimization
- Brand Monitoring
- SEO
- Competitor Analysis
- MCP
---
