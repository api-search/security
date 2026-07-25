---
api_key_in:
- header
api_specs:
- filename: panther-alert-api-openapi.yml
  format: yaml
  label: Panther alert API
  slug: panther-alert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-alert-api-openapi.yml
- filename: panther-api-token-api-openapi.yml
  format: yaml
  label: Panther api token API
  slug: panther-api-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-api-token-api-openapi.yml
- filename: panther-aws-cloud-account-api-openapi.yml
  format: yaml
  label: Panther aws cloud account API
  slug: panther-aws-cloud-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-aws-cloud-account-api-openapi.yml
- filename: panther-comment-api-openapi.yml
  format: yaml
  label: Panther comment API
  slug: panther-comment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-comment-api-openapi.yml
- filename: panther-contexttag-api-openapi.yml
  format: yaml
  label: Panther contexttag API
  slug: panther-contexttag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-contexttag-api-openapi.yml
- filename: panther-correlation-rule-api-openapi.yml
  format: yaml
  label: Panther correlation rule API
  slug: panther-correlation-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-correlation-rule-api-openapi.yml
- filename: panther-data-model-api-openapi.yml
  format: yaml
  label: Panther data model API
  slug: panther-data-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-data-model-api-openapi.yml
- filename: panther-gcs-source-api-openapi.yml
  format: yaml
  label: Panther gcs source API
  slug: panther-gcs-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-gcs-source-api-openapi.yml
- filename: panther-global-api-openapi.yml
  format: yaml
  label: Panther global API
  slug: panther-global-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-global-api-openapi.yml
- filename: panther-http-source-api-openapi.yml
  format: yaml
  label: Panther http source API
  slug: panther-http-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-http-source-api-openapi.yml
- filename: panther-log-forwarder-source-api-openapi.yml
  format: yaml
  label: Panther log forwarder source API
  slug: panther-log-forwarder-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-log-forwarder-source-api-openapi.yml
- filename: panther-log-source-alarm-api-openapi.yml
  format: yaml
  label: Panther log source alarm API
  slug: panther-log-source-alarm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-log-source-alarm-api-openapi.yml
- filename: panther-policy-api-openapi.yml
  format: yaml
  label: Panther policy API
  slug: panther-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-policy-api-openapi.yml
- filename: panther-pub-sub-source-api-openapi.yml
  format: yaml
  label: Panther pub/sub source API
  slug: panther-pub-sub-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-pub-sub-source-api-openapi.yml
- filename: panther-query-api-openapi.yml
  format: yaml
  label: Panther query API
  slug: panther-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-query-api-openapi.yml
- filename: panther-role-api-openapi.yml
  format: yaml
  label: Panther role API
  slug: panther-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-role-api-openapi.yml
- filename: panther-rule-api-openapi.yml
  format: yaml
  label: Panther rule API
  slug: panther-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-rule-api-openapi.yml
- filename: panther-s3-source-api-openapi.yml
  format: yaml
  label: Panther s3 source API
  slug: panther-s3-source-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-s3-source-api-openapi.yml
- filename: panther-scheduled-rule-api-openapi.yml
  format: yaml
  label: Panther scheduled rule API
  slug: panther-scheduled-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-scheduled-rule-api-openapi.yml
- filename: panther-simple-rule-api-openapi.yml
  format: yaml
  label: Panther simple rule API
  slug: panther-simple-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-simple-rule-api-openapi.yml
- filename: panther-user-api-openapi.yml
  format: yaml
  label: Panther user API
  slug: panther-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/panther/refs/heads/main/openapi/panther-user-api-openapi.yml
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
