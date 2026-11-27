---
anonymous_access: false
api_key_in: []
api_specs:
- filename: causeriebot-com-chatbots-api-openapi.yml
  format: yaml
  label: Causerie Chatbots API
  slug: causeriebot-com-chatbots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/causeriebot-com/openapi/causeriebot-com-chatbots-api-openapi.yml
- filename: causeriebot-com-conversations-api-openapi.yml
  format: yaml
  label: Causerie Conversations API
  slug: causeriebot-com-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/causeriebot-com/openapi/causeriebot-com-conversations-api-openapi.yml
- filename: causeriebot-com-leads-api-openapi.yml
  format: yaml
  label: Causerie Leads API
  slug: causeriebot-com-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/causeriebot-com/openapi/causeriebot-com-leads-api-openapi.yml
auth_types: []
description: Authentication for Causerie API uses a personal API key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Causerie Authentication
name_suffix: Authentication
oauth_flows: []
overview: Causerie declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Causerie
provider_slug: causeriebot-com
scheme_count: 1
schemes:
- evidence: 'Le serveur attend Authorization: Bearer VOTRE_CLE : sans le mot Bearer, avec deux espaces, ou dans un autre en-tête, le jeton n’est pas lu.'
  header: Authorization
  how_to_obtain: Generate a personal API key in the dashboard and copy it.
  location: header
  name: Bearer token
  type: http-bearer
slug: causeriebot-com-authentication
source_filename: causeriebot-com-authentication.yml
source_heading: Authentication Profile
source_url: https://causeriebot.com/docs/erreur-invalid-token/
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://causeriebot.com/docs/erreur-invalid-token/\nsources:\n- https://causeriebot.com/docs/erreur-invalid-token/\ndescription: Authentication for Causerie API uses a personal API key sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Le serveur attend Authorization: Bearer VOTRE_CLE : sans le mot Bearer, avec deux espaces, ou dans un autre en-tête, le jeton n’est\n    pas lu.'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a personal API key in the dashboard and copy it.\ndocs: https://causeriebot.com/docs/erreur-invalid-token/\n"
source_yaml_url: https://artifacts.apis.io/causeriebot-com/authentication/causeriebot-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Chatbots
- Customer Service
- Lead Qualification
- French
---
