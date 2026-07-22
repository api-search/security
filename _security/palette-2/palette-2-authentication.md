---
api_key_in: []
auth_types:
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Palette 2 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Palette 2 secures its APIs with apiKey and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Palette 2
provider_slug: palette-2
scheme_count: 2
schemes:
- description: Palette's developer API is accessed with an API key generated and managed from the Studio profile (https://studio.palettetechnology.com/profile). Requests to the base path https://studio.palettetechnology.com/api/v1 return HTTP 401 when unauthenticated, confirming API-key-gated access. The exact header name and prefix were not published in developer docs at the time of profiling.
  in: header
  name: apiKey
  sources:
  - https://palettetechnology.com/
  - probe:https://studio.palettetechnology.com/api/v1
  type: apiKey
- description: The Palette application supports enterprise single sign-on via SAML and OIDC with MFA, per the published security page. This governs interactive user access to the Studio; programmatic API access uses API keys.
  name: sso
  sources:
  - https://palettetechnology.com/security
  type: openIdConnect
slug: palette-2-authentication
source_filename: palette-2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://palettetechnology.com/ (developer/API-key management), https://palettetechnology.com/security, live probe of https://studio.palettetechnology.com/api/v1\nsummary:\n  types:\n  - apiKey\n  - openIdConnect\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  description: >-\n    Palette's developer API is accessed with an API key generated and managed\n    from the Studio profile (https://studio.palettetechnology.com/profile).\n    Requests to the base path https://studio.palettetechnology.com/api/v1\n    return HTTP 401 when unauthenticated, confirming API-key-gated access. The\n    exact header name and prefix were not published in developer docs at the\n    time of profiling.\n  sources:\n  - https://palettetechnology.com/\n  - probe:https://studio.palettetechnology.com/api/v1\n- name: sso\n  type: openIdConnect\n  description: >-\n    The Palette application supports enterprise single sign-on via SAML and\n\
  \    OIDC with MFA, per the published security page. This governs interactive\n    user access to the Studio; programmatic API access uses API keys.\n  sources:\n  - https://palettetechnology.com/security\nnotes:\n- No public OpenAPI or developer reference was available; auth profile is\n  derived from the marketing/security pages and a live 401 probe of the API\n  base path, not from a machine-readable specification.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/palette-2/refs/heads/main/authentication/palette-2-authentication.yml
summary_line: apiKey/openIdConnect · 2 schemes
tags:
- Company
- Artificial Intelligence
- Generative AI
- Video Generation
- Media
- Content Generation
- Multimodal
- Creative Tools
---
