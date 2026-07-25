---
api_key_in: []
api_specs:
- filename: ada-subpackage-channels-api-openapi.yml
  format: yaml
  label: Ada subpackage_channels API
  slug: ada-subpackage-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-channels-api-openapi.yml
- filename: ada-subpackage-conversations-api-openapi.yml
  format: yaml
  label: Ada subpackage_conversations API
  slug: ada-subpackage-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-conversations-api-openapi.yml
- filename: ada-subpackage-deletechatterdata-api-openapi.yml
  format: yaml
  label: Ada subpackage_deleteChatterData API
  slug: ada-subpackage-deletechatterdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-deletechatterdata-api-openapi.yml
- filename: ada-subpackage-endusers-api-openapi.yml
  format: yaml
  label: Ada subpackage_endUsers API
  slug: ada-subpackage-endusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-endusers-api-openapi.yml
- filename: ada-subpackage-knowledge-subpackage-knowledge-articles-api-openapi.yml
  format: yaml
  label: Ada subpackage_knowledge.subpackage_knowledge/articles API
  slug: ada-subpackage-knowledge-subpackage-knowledge-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-knowledge-subpackage-knowledge-articles-api-openapi.yml
- filename: ada-subpackage-knowledge-subpackage-knowledge-sources-api-openapi.yml
  format: yaml
  label: Ada subpackage_knowledge.subpackage_knowledge/sources API
  slug: ada-subpackage-knowledge-subpackage-knowledge-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-knowledge-subpackage-knowledge-sources-api-openapi.yml
- filename: ada-subpackage-knowledge-subpackage-knowledge-tags-api-openapi.yml
  format: yaml
  label: Ada subpackage_knowledge.subpackage_knowledge/tags API
  slug: ada-subpackage-knowledge-subpackage-knowledge-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-knowledge-subpackage-knowledge-tags-api-openapi.yml
- filename: ada-subpackage-messages-api-openapi.yml
  format: yaml
  label: Ada subpackage_messages API
  slug: ada-subpackage-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-messages-api-openapi.yml
- filename: ada-subpackage-platformintegrations-api-openapi.yml
  format: yaml
  label: Ada subpackage_platformIntegrations API
  slug: ada-subpackage-platformintegrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-platformintegrations-api-openapi.yml
- filename: ada-subpackage-webhookmanagement-api-openapi.yml
  format: yaml
  label: Ada subpackage_webhookManagement API
  slug: ada-subpackage-webhookmanagement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/openapi/ada-subpackage-webhookmanagement-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ada Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ada secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ada
provider_slug: ada
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ada-data-compliance-openapi.yml
  - openapi/ada-data-export-openapi.yml
  - openapi/ada-data-export-v1-4-openapi.yml
  - openapi/ada-knowledge-openapi.yml
  type: http
slug: ada-authentication
source_filename: ada-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ada-data-compliance-openapi.yml, openapi/ada-data-export-openapi.yml, openapi/ada-data-export-v1-4-openapi.yml,\n  openapi/ada-knowledge-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ada-data-compliance-openapi.yml\n  - openapi/ada-data-export-openapi.yml\n  - openapi/ada-data-export-v1-4-openapi.yml\n  - openapi/ada-knowledge-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ada/refs/heads/main/authentication/ada-authentication.yml
summary_line: http · 1 scheme
tags:
- ai
- customer-service
- chatbot
- automation
- conversational-ai
- helpdesk
- crm
- integrations
- knowledge-management
- data-export
---
