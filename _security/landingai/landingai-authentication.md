---
api_key_in: []
api_specs:
- filename: landingai-ade-v2-openapi-original.json
  format: json
  label: LandingAI Agentic Document Extraction (ADE) API v2
  slug: ade-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-ade-v2-openapi-original.json
- filename: landingai-ade-v1-openapi-original.json
  format: json
  label: LandingAI Agentic Document Extraction (ADE) API v1
  slug: ade-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-ade-v1-openapi-original.json
- filename: landingai-vision-tools-openapi-original.json
  format: json
  label: LandingAI Vision Tools API
  slug: vision-tools
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-vision-tools-openapi-original.json
- filename: landingai-landinglens-openapi-original.json
  format: json
  label: LandingLens API
  slug: landinglens
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/openapi/landingai-landinglens-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Landingai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Landing.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Landing.ai
provider_slug: landingai
scheme_count: 1
schemes:
- bearerFormat: Basic
  description: 'Your unique API key for authentication. Get your API key here: https://va.landing.ai/settings/api-key. If using the EU endpoint, get your API key here: https://va.eu-west-1.landing.ai/settings/api-key.'
  header: Authorization
  name: Basic Auth
  naming_note: 'The scheme is named "Basic Auth" and declares bearerFormat "Basic" in the published specs, but its type/scheme is http/bearer and the documented usage is an Authorization: Bearer header. The name is a misnomer in the provider''s spec, not actual HTTP Basic authentication — this is a good candidate for a spec-quality issue to file upstream.'
  scheme: bearer
  sources:
  - openapi/landingai-ade-v1-openapi-original.json
  - openapi/landingai-vision-tools-openapi-original.json
  type: http
  value_format: Bearer <API_KEY>
slug: landingai-authentication
source_filename: landingai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/landingai-ade-v1-openapi-original.json, openapi/landingai-vision-tools-openapi-original.json\ndocs: https://docs.landing.ai/dpt3/agentic-api-key\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\n  oauth: false\n  note: >-\n    LandingAI ADE authenticates with a single API key presented as an HTTP bearer\n    token. There is no OAuth 2.0 authorization surface and therefore no scope\n    model, so no scopes/ artifact is produced for this provider. SAML 2.0 and\n    OpenID Connect exist only as SSO into the ADE web application on Enterprise\n    plans, not as an API authorization mechanism.\nschemes:\n- name: Basic Auth\n  type: http\n  scheme: bearer\n  bearerFormat: Basic\n  description: >-\n    Your unique API key for authentication. Get your API key here:\n    https://va.landing.ai/settings/api-key. If using the EU endpoint, get your\n    API key here: https://va.eu-west-1.landing.ai/settings/api-key.\n\
  \  header: Authorization\n  value_format: Bearer <API_KEY>\n  sources:\n  - openapi/landingai-ade-v1-openapi-original.json\n  - openapi/landingai-vision-tools-openapi-original.json\n  naming_note: >-\n    The scheme is named \"Basic Auth\" and declares bearerFormat \"Basic\" in the\n    published specs, but its type/scheme is http/bearer and the documented usage\n    is an Authorization: Bearer header. The name is a misnomer in the provider's\n    spec, not actual HTTP Basic authentication — this is a good candidate for a\n    spec-quality issue to file upstream.\nspec_gaps:\n- spec: openapi/landingai-ade-v2-openapi-original.json\n  gap: >-\n    The curated ADE v2 OpenAPI declares no components.securitySchemes and no\n    security requirement, even though the documented v2 API requires the same\n    bearer API key. Captured in overlays/landingai-ade-v2-overlay.yaml.\n- spec: openapi/landingai-landinglens-openapi-original.json\n  gap: >-\n    The LandingLens OpenAPI declares no components.securitySchemes,\
  \ though the\n    API requires an API key.\nkey_management:\n  us: https://ade.landing.ai/\n  eu: https://va.eu-west-1.landing.ai/settings/api-key\n  docs: https://docs.landing.ai/dpt3/agentic-api-key\nsso:\n  supported: true\n  scope: ADE web application (Enterprise plans), not API authorization\n  protocols: [SAML 2.0, OpenID Connect]\n  docs: https://docs.landing.ai/ade/ade-sso\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landingai/refs/heads/main/authentication/landingai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Document Extraction
- Document Processing
- Computer Vision
- OCR
- Data Extraction
- Agents
- Developer Tools
---
