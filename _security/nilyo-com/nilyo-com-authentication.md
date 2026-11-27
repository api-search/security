---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nilyo-com-openapi-generated.yml
  format: yaml
  label: nilyo-com API
  slug: nilyo-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nilyo-com/openapi/_ae-authored/nilyo-com-openapi-generated.yml
auth_types: []
description: Authentication methods published by Nilyo
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: nilyo-com Authentication
name_suffix: Authentication
oauth_flows: []
overview: nilyo-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: nilyo-com
provider_slug: nilyo-com
scheme_count: 2
schemes:
- evidence: 'Signing in: OAuth 2.1, no shared passwords'
  how_to_obtain: When you add Nilyo to an agent, the agent registers itself with Nilyo (dynamic client registration) and sends you to nilyo.com to sign in or create your account.
  name: OAuth 2.1
  type: oauth2
- evidence: Create a personal token in Nilyo under Agent access and store it in a credential named Nilyo API.
  how_to_obtain: Create a personal token in Nilyo under Agent access and store it in a credential named Nilyo API.
  name: Personal token
  type: apiKey
slug: nilyo-com-authentication
source_filename: nilyo-com-authentication.yml
source_heading: Authentication Profile
source_url: https://nilyo.com/how-it-works
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nilyo.com/how-it-works\nsources:\n- https://nilyo.com/how-it-works\n- https://nilyo.com/guides/connect-telegram-to-n8n\n- https://nilyo.com/setup-for-agents\n- https://nilyo.com/agents/grok\ndescription: Authentication methods published by Nilyo\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: 'Signing in: OAuth 2.1, no shared passwords'\n  how_to_obtain: When you add Nilyo to an agent, the agent registers itself with Nilyo (dynamic client registration) and sends you to nilyo.com\n    to sign in or create your account.\n- type: apiKey\n  name: Personal token\n  evidence: Create a personal token in Nilyo under Agent access and store it in a credential named Nilyo API.\n  how_to_obtain: Create a personal token in Nilyo under Agent access and store it in a credential named Nilyo API.\ndocs: https://nilyo.com/how-it-works\n"
source_yaml_url: https://artifacts.apis.io/nilyo-com/authentication/nilyo-com-authentication.yml
summary_line: 2 schemes
tags:
- Integration
- AI Agents
- Messaging
- LinkedIn
- WhatsApp
- Email
- ChatGPT
- Claude
---
