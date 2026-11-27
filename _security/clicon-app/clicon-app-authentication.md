---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clicon-app-openapi-generated.yml
  format: yaml
  label: Clicon Lotus Bot Tracking API
  slug: clicon-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clicon-app/openapi/_ae-authored/clicon-app-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Clicon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Clicon declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Clicon
provider_slug: clicon-app
scheme_count: 1
schemes:
- applies_to:
  - Lotus MCP server (https://lotus.clicon.app/mcp/)
  - POST https://lotus.clicon.app/api/v1/track/bot-hit
  evidence:
  - quote: Invalid API key Check your API key in the Lotus admin panel. Keys start with lotus_pk_.
    source: https://clicon.app/en/integrations/mcp
  - quote: You can find your key in the Lotus admin panel under Settings → API Keys. The middleware uses this key to authenticate tracking requests to the Lotus API.
    source: https://clicon.app/en/docs/bot-tracking
  failure: Getting 401 from tracking endpoint Your LOTUS_TRACKING_KEY is invalid or expired.
  header: X-API-Key
  in: header
  key_prefix: lotus_pk_
  name: X-API-Key
  type: apiKey
slug: clicon-app-authentication
source_filename: clicon-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://clicon.app/en/integrations/mcp\ndocs: https://clicon.app/en/integrations/mcp\nsee_also:\n- https://clicon.app/en/docs/bot-tracking\nnote: The generated OpenAPI declares no securitySchemes; both docs pages state an X-API-Key header. Keys are issued from the Lotus admin panel to account holders (no self-serve signup; access via demo request).\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  header: X-API-Key\n  applies_to:\n  - Lotus MCP server (https://lotus.clicon.app/mcp/)\n  - POST https://lotus.clicon.app/api/v1/track/bot-hit\n  key_prefix: lotus_pk_\n  evidence:\n  - quote: \"Invalid API key Check your API key in the Lotus admin panel. Keys start with lotus_pk_.\"\n    source: https://clicon.app/en/integrations/mcp\n  - quote: \"You can find your key in the Lotus admin panel under Settings → API Keys. The middleware uses this key to authenticate tracking requests to the Lotus API.\"\n    source: https://clicon.app/en/docs/bot-tracking\n\
  \  failure: \"Getting 401 from tracking endpoint Your LOTUS_TRACKING_KEY is invalid or expired.\"\n"
source_yaml_url: https://artifacts.apis.io/clicon-app/authentication/clicon-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Generative Engine Optimization
- MCP
- AI Crawlers
- Analytics
- BusinessTools
- SEO
---
