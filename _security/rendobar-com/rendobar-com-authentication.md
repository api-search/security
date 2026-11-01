---
anonymous_access: false
api_key_in: []
api_specs:
- filename: rendobar-com-account-api-openapi.yml
  format: yaml
  label: rendobar-com Account API
  slug: rendobar-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-account-api-openapi.yml
- filename: rendobar-com-api-keys-api-openapi.yml
  format: yaml
  label: rendobar-com API Keys API
  slug: rendobar-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-api-keys-api-openapi.yml
- filename: rendobar-com-assets-api-openapi.yml
  format: yaml
  label: rendobar-com Assets API
  slug: rendobar-com-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-assets-api-openapi.yml
- filename: rendobar-com-billing-api-openapi.yml
  format: yaml
  label: rendobar-com Billing API
  slug: rendobar-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-billing-api-openapi.yml
- filename: rendobar-com-compose-api-openapi.yml
  format: yaml
  label: rendobar-com Compose API
  slug: rendobar-com-compose-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-compose-api-openapi.yml
- filename: rendobar-com-jobs-api-openapi.yml
  format: yaml
  label: rendobar-com Jobs API
  slug: rendobar-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-jobs-api-openapi.yml
- filename: rendobar-com-models-api-openapi.yml
  format: yaml
  label: rendobar-com Models API
  slug: rendobar-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-models-api-openapi.yml
- filename: rendobar-com-notifications-api-openapi.yml
  format: yaml
  label: rendobar-com Notifications API
  slug: rendobar-com-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-notifications-api-openapi.yml
- filename: rendobar-com-organizations-api-openapi.yml
  format: yaml
  label: rendobar-com Organizations API
  slug: rendobar-com-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-organizations-api-openapi.yml
- filename: rendobar-com-sharing-api-openapi.yml
  format: yaml
  label: rendobar-com Sharing API
  slug: rendobar-com-sharing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-sharing-api-openapi.yml
- filename: rendobar-com-storage-api-openapi.yml
  format: yaml
  label: rendobar-com Storage API
  slug: rendobar-com-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-storage-api-openapi.yml
- filename: rendobar-com-team-api-openapi.yml
  format: yaml
  label: rendobar-com Team API
  slug: rendobar-com-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-team-api-openapi.yml
- filename: rendobar-com-upload-sessions-api-openapi.yml
  format: yaml
  label: rendobar-com Upload Sessions API
  slug: rendobar-com-upload-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-upload-sessions-api-openapi.yml
- filename: rendobar-com-webhooks-api-openapi.yml
  format: yaml
  label: rendobar-com Webhooks API
  slug: rendobar-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rendobar-com/openapi/rendobar-com-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Rendobar Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: rendobar-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: rendobar-com
provider_slug: rendobar-com
scheme_count: 2
schemes:
- bearerFormat: API key or OAuth access token
  description: Bearer authentication using API key (rb_...) or OAuth 2.1 token.
  in: header
  name: Authorization
  scheme: bearer
  type: http
- description: OAuth 2.1 with PKCE. Register a client at https://api.rendobar.com/oauth2/register.
  flows:
    authorizationCode:
      authorizationUrl: https://api.rendobar.com/auth/oauth2/authorize
      refreshUrl: https://api.rendobar.com/auth/oauth2/token
      scopes:
        assets:read: See and download your files
        assets:write: Upload and delete files
        billing:read: See your plan, balance and usage
        billing:write: Change your plan and payment methods
        jobs:read: See your jobs and their results
        jobs:write: Run and cancel jobs
        keys:read: See which API keys exist
        keys:write: Create and revoke API keys
        orgs:read: See your organization and its members
        orgs:write: Manage your organization and its members
        storage:read: See which storage connections exist
        storage:write: Connect, rotate and remove storage connections
        webhooks:read: See where your events are delivered
        webhooks:write: Manage where your events are delivered
      tokenUrl: https://api.rendobar.com/auth/oauth2/token
  type: oauth2
slug: rendobar-com-authentication
source_filename: rendobar-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: https://api.rendobar.com/openapi.json\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: API key or OAuth access token\n    description: Bearer authentication using API key (rb_...) or OAuth 2.1 token.\n    name: Authorization\n    in: header\n  - type: oauth2\n    description: OAuth 2.1 with PKCE. Register a client at https://api.rendobar.com/oauth2/register.\n    flows:\n      authorizationCode:\n        authorizationUrl: https://api.rendobar.com/auth/oauth2/authorize\n        tokenUrl: https://api.rendobar.com/auth/oauth2/token\n        refreshUrl: https://api.rendobar.com/auth/oauth2/token\n        scopes:\n          jobs:read: See your jobs and their results\n          jobs:write: Run and cancel jobs\n          assets:read: See and download your files\n          assets:write: Upload and delete files\n          webhooks:read: See where your events are delivered\n          webhooks:write: Manage where your events\
  \ are delivered\n          billing:read: See your plan, balance and usage\n          billing:write: Change your plan and payment methods\n          orgs:read: See your organization and its members\n          orgs:write: Manage your organization and its members\n          keys:read: See which API keys exist\n          keys:write: Create and revoke API keys\n          storage:read: See which storage connections exist\n          storage:write: Connect, rotate and remove storage connections\n"
source_yaml_url: https://artifacts.apis.io/rendobar-com/authentication/rendobar-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- VideoProcessing
- FFmpeg
- AI
- Serverless
- MediaAPI
---
