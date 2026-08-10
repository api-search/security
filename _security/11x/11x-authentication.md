---
api_key_in:
- query
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: 11X Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: 11x secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: 11x
provider_slug: 11x
scheme_count: 2
schemes:
- description: An 11x key passed as the `apikey` query parameter when loading the PersonaClient browser script, and again to the PersonaClient constructor. This is the only 11x authentication mechanism observed in published documentation. Note it is a browser-side key embedded in page markup, so it is a publishable client-side identifier rather than a secret.
  documented_example: script.src = "https://api.prod.centralus.az.sindarin.tech/PersonaClientPublicV2?apikey=<YOUR_11X_KEY>"
  in: query
  name: 11xApiKey
  parameter: apikey
  sources:
  - https://11x.mintlify.app/integrations/mike-browser-implementation
  surface: browser embed
  type: apiKey
- broker: Ampersand
  description: CRM connections (Salesforce, HubSpot, Zoho) are established over "a secure OAuth connection" brokered by Ampersand. The end user authorizes in-browser from the 11x integrations tab; 11x publishes no client credentials, endpoints, or scope list for this flow.
  flows:
  - authorizationUrl: null
    flow: authorizationCode
    tokenUrl: null
  name: CrmOAuth
  providers:
  - salesforce
  - hubspot
  - zoho
  sources:
  - https://11x.mintlify.app/integrations/mike-crm-integration
  type: oauth2
slug: 11x-authentication
source_filename: 11x-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://11x.mintlify.app/integrations/mike-browser-implementation\ndocs: https://11x.mintlify.app/integrations/mike-browser-implementation\nspec_derived: false\nspec_note: >-\n  derive-authentication.py was not run: there is no OpenAPI/Swagger in this repo and none is\n  published by 11x, so there are no securitySchemes to aggregate. Everything below was read from\n  11x's published documentation, not inferred.\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [query]\n  oauth2_flows: [authorizationCode]\n  oauth2_delegated_to: Ampersand (third-party integration broker)\nschemes:\n- name: 11xApiKey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: >-\n    An 11x key passed as the `apikey` query parameter when loading the PersonaClient browser\n    script, and again to the PersonaClient constructor. This is the only 11x authentication\n    mechanism observed in published documentation. Note it is a browser-side\
  \ key embedded in\n    page markup, so it is a publishable client-side identifier rather than a secret.\n  surface: browser embed\n  documented_example: 'script.src = \"https://api.prod.centralus.az.sindarin.tech/PersonaClientPublicV2?apikey=<YOUR_11X_KEY>\"'\n  sources:\n  - https://11x.mintlify.app/integrations/mike-browser-implementation\n- name: CrmOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: null\n    tokenUrl: null\n  description: >-\n    CRM connections (Salesforce, HubSpot, Zoho) are established over \"a secure OAuth connection\"\n    brokered by Ampersand. The end user authorizes in-browser from the 11x integrations tab; 11x\n    publishes no client credentials, endpoints, or scope list for this flow.\n  broker: Ampersand\n  providers: [salesforce, hubspot, zoho]\n  sources:\n  - https://11x.mintlify.app/integrations/mike-crm-integration\nplatform_api:\n  documented: false\n  note: >-\n    The 11x Platform API marketed at /platform/integrations/api\
  \ publishes no authentication\n    documentation. api.11x.ai returns HTTP 403 to every anonymous request, including\n    /.well-known/ paths, so no auth challenge, WWW-Authenticate header, or OAuth metadata could\n    be observed.\nunverified_claims:\n- claim: 'Authorization: Bearer YOUR_API_KEY'\n  source: https://11x.mintlify.app/.well-known/agent-skills/11x/skill.md\n  verified: false\n  note: >-\n    Appears in 11x's published agent skill, but that document is machine-generated boilerplate\n    that misdescribes 11x as an RPA platform and lists explicitly hypothetical endpoints. NOT\n    treated as a verified 11x auth scheme.\nx-evidence:\n  fetched: '2026-08-05'\n  probes:\n  - {url: 'https://api.11x.ai/.well-known/openid-configuration', http_status: 403}\n  - {url: 'https://api.11x.ai/.well-known/oauth-authorization-server', http_status: 403}\n  - {url: 'https://www.11x.ai/.well-known/openid-configuration', http_status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/11x/refs/heads/main/authentication/11x-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Artificial Intelligence
- AI Agents
- Sales
- Sales Automation
- Lead Generation
- Conversational AI
- Voice
- CRM
- Go To Market
---
