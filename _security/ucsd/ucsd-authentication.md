---
api_key_in: []
api_specs:
- filename: ucsd-chat-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — chat
  slug: tritonai-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-chat-api-openapi.yml
- filename: ucsd-completions-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — completions
  slug: tritonai-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-completions-api-openapi.yml
- filename: ucsd-embeddings-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — embeddings
  slug: tritonai-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-embeddings-api-openapi.yml
- filename: ucsd-models-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — models
  slug: tritonai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-models-api-openapi.yml
- filename: ucsd-images-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — images
  slug: tritonai-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-images-api-openapi.yml
- filename: ucsd-audio-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — audio
  slug: tritonai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-audio-api-openapi.yml
- filename: ucsd-scim-api-openapi.yml
  format: yaml
  label: TritonAI Developer API — SCIM 2.0 provisioning
  slug: tritonai-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-scim-api-openapi.yml
- filename: ucsd-library-digital-collections-openapi.yml
  format: yaml
  label: UC San Diego Library Digital Collections JSON API
  slug: library-digital-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/openapi/ucsd-library-digital-collections-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ucsd Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of California, San Diego secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of California, San Diego
provider_slug: ucsd
scheme_count: 1
schemes:
- description: Issued TritonAI API key passed as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_original/ucsd-tritonai.yaml
  type: http
slug: ucsd-authentication
source_filename: ucsd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/_original/ucsd-tritonai.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Issued TritonAI API key passed as a Bearer token.\n  sources:\n  - openapi/_original/ucsd-tritonai.yaml\nsurfaces:\n- name: TritonAI Developer API (LiteLLM Gateway)\n  host: tritonai-api.ucsd.edu\n  x-operator: institution\n  scheme: bearerAuth\n  method: derived\n  source: openapi/_original/ucsd-tritonai.yaml\n- name: UC San Diego API Gateway (WSO2 API Manager 4.1.0)\n  host: api.ucsd.edu\n  x-operator: institution\n  scheme: OAuth 2.0 / OpenID Connect via the gateway's internal key manager\n  method: probed\n  source: https://api.ucsd.edu/api/am/devportal/v2/settings\n  notes: >-\n    IsAnonymousModeEnabled=false and identityProvider.external=false; the API catalogue returns\n    401 to anonymous clients. Credentials are issued to UC San Diego affiliates through Single\n    Sign-On,\
  \ not through self-serve registration. See scopes/ucsd-scopes.yml.\n- name: UC San Diego Shibboleth Identity Provider (TritON)\n  host: a5.ucsd.edu\n  x-operator: institution\n  scheme: SAML 2.0 Web Browser SSO — HTTP-POST and HTTP-Redirect bindings\n  method: probed\n  source: https://mdq.incommon.org/entities/urn%3Amace%3Aincommon%3Aucsd.edu\n  notes: >-\n    Registered in InCommon (and via InCommon in eduGAIN) as urn:mace:incommon:ucsd.edu. This is\n    the authentication layer behind nearly every gated campus API.\n- name: UC San Diego Library Digital Collections JSON API\n  host: library.ucsd.edu\n  x-operator: institution\n  scheme: none — anonymous read\n  method: probed\n  source: https://library.ucsd.edu/dc/search.json?q=ocean\n  notes: >-\n    No authorization layer. Access control is enforced server-side by a fixed Solr filter query\n    on discover_access_group_ssim.\n- name: UC San Diego Web API Portal\n  host: collab.ucsd.edu\n  x-operator: tenant\n  scheme: Atlassian Confluence\
  \ Cloud SSO\n  method: probed\n  source: https://collab.ucsd.edu/api/api-documentation\n  notes: >-\n    302 to ucsdcollab.atlassian.net/wiki. The documentation is gated by the Atlassian tenant's\n    own SSO, not by a UC San Diego API authorization layer.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucsd/refs/heads/main/authentication/ucsd-authentication.yml
summary_line: http · 1 scheme
tags:
- Education
- Higher Education
- University
- Public Research University
- UC System
- United States
- California
- Research
- Research Data
- Digital Collections
- Identity Federation
- API Gateway
- Artificial Intelligence
- Research Computing
---
