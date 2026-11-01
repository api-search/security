---
anonymous_access: false
api_key_in: []
api_specs:
- filename: actionbox-cloud-account-api-openapi.yml
  format: yaml
  label: actionbox-cloud Account API
  slug: actionbox-cloud-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-account-api-openapi.yml
- filename: actionbox-cloud-actions-api-openapi.yml
  format: yaml
  label: actionbox-cloud Actions API
  slug: actionbox-cloud-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-actions-api-openapi.yml
- filename: actionbox-cloud-analytics-api-openapi.yml
  format: yaml
  label: actionbox-cloud Analytics API
  slug: actionbox-cloud-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-analytics-api-openapi.yml
- filename: actionbox-cloud-auth-api-openapi.yml
  format: yaml
  label: actionbox-cloud Auth API
  slug: actionbox-cloud-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-auth-api-openapi.yml
- filename: actionbox-cloud-billing-api-openapi.yml
  format: yaml
  label: actionbox-cloud Billing API
  slug: actionbox-cloud-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-billing-api-openapi.yml
- filename: actionbox-cloud-dashboard-api-openapi.yml
  format: yaml
  label: actionbox-cloud Dashboard API
  slug: actionbox-cloud-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-dashboard-api-openapi.yml
- filename: actionbox-cloud-devices-api-openapi.yml
  format: yaml
  label: actionbox-cloud Devices API
  slug: actionbox-cloud-devices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-devices-api-openapi.yml
- filename: actionbox-cloud-documentation-api-openapi.yml
  format: yaml
  label: actionbox-cloud Documentation API
  slug: actionbox-cloud-documentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-documentation-api-openapi.yml
- filename: actionbox-cloud-feedback-api-openapi.yml
  format: yaml
  label: actionbox-cloud Feedback API
  slug: actionbox-cloud-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-feedback-api-openapi.yml
- filename: actionbox-cloud-notifications-api-openapi.yml
  format: yaml
  label: actionbox-cloud Notifications API
  slug: actionbox-cloud-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-notifications-api-openapi.yml
- filename: actionbox-cloud-runs-api-openapi.yml
  format: yaml
  label: actionbox-cloud Runs API
  slug: actionbox-cloud-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-runs-api-openapi.yml
- filename: actionbox-cloud-slack-api-openapi.yml
  format: yaml
  label: actionbox-cloud Slack API
  slug: actionbox-cloud-slack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-slack-api-openapi.yml
- filename: actionbox-cloud-sources-api-openapi.yml
  format: yaml
  label: actionbox-cloud Sources API
  slug: actionbox-cloud-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-sources-api-openapi.yml
- filename: actionbox-cloud-system-api-openapi.yml
  format: yaml
  label: actionbox-cloud System API
  slug: actionbox-cloud-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-system-api-openapi.yml
- filename: actionbox-cloud-watches-api-openapi.yml
  format: yaml
  label: actionbox-cloud Watches API
  slug: actionbox-cloud-watches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-watches-api-openapi.yml
- filename: actionbox-cloud-webhooks-api-openapi.yml
  format: yaml
  label: actionbox-cloud Webhooks API
  slug: actionbox-cloud-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-webhooks-api-openapi.yml
- filename: actionbox-cloud-workspaces-api-openapi.yml
  format: yaml
  label: actionbox-cloud Workspaces API
  slug: actionbox-cloud-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/actionbox-cloud/openapi/actionbox-cloud-workspaces-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Actionbox Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: actionbox-cloud declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: actionbox-cloud
provider_slug: actionbox-cloud
scheme_count: 2
schemes:
- description: Source API key (`axb_live_…`) used for machine integrations.
  name: SourceBearer
  scheme: bearer
  type: http
- description: User session bearer token (`axb_usr_…`).
  name: UserBearer
  scheme: bearer
  type: http
slug: actionbox-cloud-authentication
source_filename: actionbox-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource:\n  - https://actionbox.cloud/docs/api-reference#authentication\n  - https://api.actionbox.cloud/openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    name: \"SourceBearer\"\n    description: \"Source API key (`axb_live_…`) used for machine integrations.\"\n  - type: http\n    scheme: bearer\n    name: \"UserBearer\"\n    description: \"User session bearer token (`axb_usr_…`).\"\n"
source_yaml_url: https://artifacts.apis.io/actionbox-cloud/authentication/actionbox-cloud-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Human-in-the-loop
- Automation
- Approval
- Cloud
---
