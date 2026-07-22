---
api_key_in:
- header
api_specs:
- filename: panther-rest-openapi.yml
  format: yaml
  label: Panther REST API
  slug: panther-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-rest-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Panther Authentication
name_suffix: Authentication
oauth_flows: []
overview: Panther secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Panther
provider_slug: panther
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/panther-rest-openapi.yml
  type: apiKey
slug: panther-authentication
source_filename: panther-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/panther-rest-openapi.yml\ndocs: https://docs.panther.com/panther-developer-workflows/api/rest/api-tokens\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nnotes: >-\n  Panther's REST API authenticates with a per-instance API token passed in the\n  X-API-Key header. Tokens are created in the Console under Settings > Developer\n  Tools > API Tokens and carry granular permission scopes (see permissions[]).\n  A token can rotate itself via POST /api-tokens/self/rotate. The Remote MCP\n  server uses OAuth 2.1 + PKCE (RFC 7591 dynamic client registration) instead of\n  a static API key.\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/panther-rest-openapi.yml\npermissions:\n- AIRunAsModify\n- AlertModify\n- AlertRead\n- BulkUpload\n- BulkUploadValidate\n- CloudsecSourceModify\n- CloudsecSourceRead\n- DataAnalyticsModify\n- DataAnalyticsRead\n- DestinationModify\n\
  - DestinationRead\n- GeneralSettingsModify\n- GeneralSettingsRead\n- LogSourceModify\n- LogSourceRawDataRead\n- LogSourceRead\n- LookupModify\n- LookupRead\n- ManageAIResponses\n- ManageAISkills\n- ManageScheduledPrompts\n- McpServerModify\n- McpServerRead\n- NotificationsSend\n- OrganizationAPITokenModify\n- OrganizationAPITokenRead\n- PolicyModify\n- PolicyRead\n- ResourceModify\n- ResourceRead\n- RuleModify\n- RuleRead\n- RunPantherAI\n- SummaryRead\n- UserModify\n- UserRead\n- ViewAIPrivateResponses\n- ViewAISkills\n- ViewScheduledPrompts\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/authentication/panther-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Security
- SIEM
- Detection and Response
- Security Operations
- Threat Detection
- Log Management
- Data Lake
- Cloud Security
- Developer Tools
---
