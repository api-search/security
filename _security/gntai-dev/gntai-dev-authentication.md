---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gntai-dev-billing-api-openapi.yml
  format: yaml
  label: gnt.ai Billing API
  slug: gntai-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-billing-api-openapi.yml
- filename: gntai-dev-brain-api-openapi.yml
  format: yaml
  label: gnt.ai Brain API
  slug: gntai-dev-brain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-brain-api-openapi.yml
- filename: gntai-dev-gaps-api-openapi.yml
  format: yaml
  label: gnt.ai Gaps API
  slug: gntai-dev-gaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-gaps-api-openapi.yml
- filename: gntai-dev-github-api-openapi.yml
  format: yaml
  label: gnt.ai GitHub API
  slug: gntai-dev-github-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-github-api-openapi.yml
- filename: gntai-dev-github-webhook-api-openapi.yml
  format: yaml
  label: gnt.ai Github Webhook API
  slug: gntai-dev-github-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-github-webhook-api-openapi.yml
- filename: gntai-dev-healthz-api-openapi.yml
  format: yaml
  label: gnt.ai Healthz API
  slug: gntai-dev-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-healthz-api-openapi.yml
- filename: gntai-dev-intercom-api-openapi.yml
  format: yaml
  label: gnt.ai Intercom API
  slug: gntai-dev-intercom-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-intercom-api-openapi.yml
- filename: gntai-dev-linear-api-openapi.yml
  format: yaml
  label: gnt.ai Linear API
  slug: gntai-dev-linear-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-linear-api-openapi.yml
- filename: gntai-dev-notion-api-openapi.yml
  format: yaml
  label: gnt.ai Notion API
  slug: gntai-dev-notion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-notion-api-openapi.yml
- filename: gntai-dev-org-admin-api-openapi.yml
  format: yaml
  label: gnt.ai Org Admin API
  slug: gntai-dev-org-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-org-admin-api-openapi.yml
- filename: gntai-dev-platform-admin-api-openapi.yml
  format: yaml
  label: gnt.ai Platform Admin API
  slug: gntai-dev-platform-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-platform-admin-api-openapi.yml
- filename: gntai-dev-roi-api-openapi.yml
  format: yaml
  label: gnt.ai Roi API
  slug: gntai-dev-roi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-roi-api-openapi.yml
- filename: gntai-dev-rules-api-openapi.yml
  format: yaml
  label: gnt.ai Rules API
  slug: gntai-dev-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-rules-api-openapi.yml
- filename: gntai-dev-settings-api-openapi.yml
  format: yaml
  label: gnt.ai Settings API
  slug: gntai-dev-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-settings-api-openapi.yml
- filename: gntai-dev-skill-packs-api-openapi.yml
  format: yaml
  label: gnt.ai Skill Packs API
  slug: gntai-dev-skill-packs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-skill-packs-api-openapi.yml
- filename: gntai-dev-slack-api-openapi.yml
  format: yaml
  label: gnt.ai Slack API
  slug: gntai-dev-slack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-slack-api-openapi.yml
- filename: gntai-dev-transcribe-api-openapi.yml
  format: yaml
  label: gnt.ai Transcribe API
  slug: gntai-dev-transcribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-transcribe-api-openapi.yml
- filename: gntai-dev-webhooks-api-openapi.yml
  format: yaml
  label: gnt.ai Webhooks API
  slug: gntai-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-webhooks-api-openapi.yml
- filename: gntai-dev-zendesk-api-openapi.yml
  format: yaml
  label: gnt.ai Zendesk API
  slug: gntai-dev-zendesk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gntai-dev/openapi/gntai-dev-zendesk-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: gnt.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: gnt.ai secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: gnt.ai
provider_slug: gntai-dev
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/gntai-dev-openapi.yml
  type: http
slug: gntai-dev-authentication
source_filename: gntai-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/gntai-dev-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/gntai-dev-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/gntai-dev/authentication/gntai-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Governance
- Compliance
- Security
- Automation
---
