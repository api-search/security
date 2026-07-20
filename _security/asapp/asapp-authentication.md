---
api_key_in:
- header
api_specs:
- filename: asapp-conversations-openapi.yml
  format: yaml
  label: ASAPP Conversations API
  slug: asapp-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-conversations-openapi.yml
- filename: asapp-generativeagent-openapi.yml
  format: yaml
  label: ASAPP GenerativeAgent API
  slug: asapp-generativeagent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-generativeagent-openapi.yml
- filename: asapp-autosummary-openapi.yml
  format: yaml
  label: ASAPP AutoSummary API
  slug: asapp-autosummary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-autosummary-openapi.yml
- filename: asapp-autocompose-openapi.yml
  format: yaml
  label: ASAPP AutoCompose API
  slug: asapp-autocompose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-autocompose-openapi.yml
- filename: asapp-autotranscribe-openapi.yml
  format: yaml
  label: ASAPP AutoTranscribe API
  slug: asapp-autotranscribe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-autotranscribe-openapi.yml
- filename: asapp-knowledge-base-openapi.yml
  format: yaml
  label: ASAPP Knowledge Base API
  slug: asapp-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-knowledge-base-openapi.yml
- filename: asapp-metadata-ingestion-openapi.yml
  format: yaml
  label: ASAPP Metadata Ingestion API
  slug: asapp-metadata-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-metadata-ingestion-openapi.yml
- filename: asapp-fileexporter-openapi.yml
  format: yaml
  label: ASAPP File Exporter API
  slug: asapp-file-exporter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-fileexporter-openapi.yml
- filename: asapp-partner-configuration-openapi.yml
  format: yaml
  label: ASAPP Partner Configuration API
  slug: asapp-partner-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-partner-configuration-openapi.yml
- filename: asapp-mg-genagent-openapi.yml
  format: yaml
  label: ASAPP GenAgent Media Gateway API
  slug: asapp-genagent-media-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-mg-genagent-openapi.yml
- filename: asapp-mg-autotranscribe-openapi.yml
  format: yaml
  label: ASAPP AutoTranscribe Media Gateway API
  slug: asapp-autotranscribe-media-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-mg-autotranscribe-openapi.yml
- filename: asapp-healthcheck-openapi.yml
  format: yaml
  label: ASAPP Health Check API
  slug: asapp-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-healthcheck-openapi.yml
- filename: asapp-openapi-openapi.yml
  format: yaml
  label: ASAPP Platform API (combined)
  slug: asapp-platform-api-combined
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/openapi/asapp-openapi-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Asapp Authentication
name_suffix: Authentication
oauth_flows: []
overview: ASAPP secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ASAPP
provider_slug: asapp
scheme_count: 2
schemes:
- in: header
  name: API-ID
  parameter: asapp-api-id
  sources:
  - openapi/asapp-autocompose-openapi.yml
  - openapi/asapp-autosummary-openapi.yml
  - openapi/asapp-autotranscribe-openapi.yml
  - openapi/asapp-conversations-openapi.yml
  - openapi/asapp-fileexporter-openapi.yml
  - openapi/asapp-generativeagent-openapi.yml
  - openapi/asapp-healthcheck-openapi.yml
  - openapi/asapp-knowledge-base-openapi.yml
  - openapi/asapp-metadata-ingestion-openapi.yml
  - openapi/asapp-mg-autotranscribe-openapi.yml
  - openapi/asapp-mg-genagent-openapi.yml
  - openapi/asapp-openapi-openapi.yml
  - openapi/asapp-partner-configuration-openapi.yml
  type: apiKey
- in: header
  name: API-Secret
  parameter: asapp-api-secret
  sources:
  - openapi/asapp-autocompose-openapi.yml
  - openapi/asapp-autosummary-openapi.yml
  - openapi/asapp-autotranscribe-openapi.yml
  - openapi/asapp-conversations-openapi.yml
  - openapi/asapp-fileexporter-openapi.yml
  - openapi/asapp-generativeagent-openapi.yml
  - openapi/asapp-healthcheck-openapi.yml
  - openapi/asapp-knowledge-base-openapi.yml
  - openapi/asapp-metadata-ingestion-openapi.yml
  - openapi/asapp-mg-autotranscribe-openapi.yml
  - openapi/asapp-mg-genagent-openapi.yml
  - openapi/asapp-openapi-openapi.yml
  - openapi/asapp-partner-configuration-openapi.yml
  type: apiKey
slug: asapp-authentication
source_filename: asapp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\ndocs: https://docs.asapp.com/getting-started/developers\nnotes: >-\n  ASAPP authenticates every request with a paired API Id and API Secret sent as\n  two headers: asapp-api-id and asapp-api-secret. Keys are issued per environment\n  (sandbox vs production). No OAuth2/OIDC surface is published. Base URLs:\n  https://api.asapp.com (production), https://api.sandbox.asapp.com (sandbox).\nsource: openapi/asapp-autocompose-openapi.yml, openapi/asapp-autosummary-openapi.yml, openapi/asapp-autotranscribe-openapi.yml,\n  openapi/asapp-conversations-openapi.yml, openapi/asapp-fileexporter-openapi.yml, openapi/asapp-generativeagent-openapi.yml,\n  openapi/asapp-healthcheck-openapi.yml, openapi/asapp-knowledge-base-openapi.yml, openapi/asapp-metadata-ingestion-openapi.yml,\n  openapi/asapp-mg-autotranscribe-openapi.yml, openapi/asapp-mg-genagent-openapi.yml, openapi/asapp-openapi-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n\
  \  - header\nschemes:\n- name: API-ID\n  type: apiKey\n  in: header\n  parameter: asapp-api-id\n  sources:\n  - openapi/asapp-autocompose-openapi.yml\n  - openapi/asapp-autosummary-openapi.yml\n  - openapi/asapp-autotranscribe-openapi.yml\n  - openapi/asapp-conversations-openapi.yml\n  - openapi/asapp-fileexporter-openapi.yml\n  - openapi/asapp-generativeagent-openapi.yml\n  - openapi/asapp-healthcheck-openapi.yml\n  - openapi/asapp-knowledge-base-openapi.yml\n  - openapi/asapp-metadata-ingestion-openapi.yml\n  - openapi/asapp-mg-autotranscribe-openapi.yml\n  - openapi/asapp-mg-genagent-openapi.yml\n  - openapi/asapp-openapi-openapi.yml\n  - openapi/asapp-partner-configuration-openapi.yml\n- name: API-Secret\n  type: apiKey\n  in: header\n  parameter: asapp-api-secret\n  sources:\n  - openapi/asapp-autocompose-openapi.yml\n  - openapi/asapp-autosummary-openapi.yml\n  - openapi/asapp-autotranscribe-openapi.yml\n  - openapi/asapp-conversations-openapi.yml\n  - openapi/asapp-fileexporter-openapi.yml\n\
  \  - openapi/asapp-generativeagent-openapi.yml\n  - openapi/asapp-healthcheck-openapi.yml\n  - openapi/asapp-knowledge-base-openapi.yml\n  - openapi/asapp-metadata-ingestion-openapi.yml\n  - openapi/asapp-mg-autotranscribe-openapi.yml\n  - openapi/asapp-mg-genagent-openapi.yml\n  - openapi/asapp-openapi-openapi.yml\n  - openapi/asapp-partner-configuration-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asapp/refs/heads/main/authentication/asapp-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- AI
- Conversational AI
- Contact Center
- Customer Experience
- Customer Service
- Generative AI
- Agent Assist
- Speech Recognition
- Knowledge Base
---
