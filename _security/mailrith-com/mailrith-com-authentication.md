---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mailrith-com-analytics-api-openapi.yml
  format: yaml
  label: Mailrith Analytics API
  slug: mailrith-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-analytics-api-openapi.yml
- filename: mailrith-com-automations-api-openapi.yml
  format: yaml
  label: Mailrith Automations API
  slug: mailrith-com-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-automations-api-openapi.yml
- filename: mailrith-com-broadcasts-api-openapi.yml
  format: yaml
  label: Mailrith Broadcasts API
  slug: mailrith-com-broadcasts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-broadcasts-api-openapi.yml
- filename: mailrith-com-custom-fields-api-openapi.yml
  format: yaml
  label: Mailrith Custom Fields API
  slug: mailrith-com-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-custom-fields-api-openapi.yml
- filename: mailrith-com-diagnostics-api-openapi.yml
  format: yaml
  label: Mailrith Diagnostics API
  slug: mailrith-com-diagnostics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-diagnostics-api-openapi.yml
- filename: mailrith-com-email-templates-api-openapi.yml
  format: yaml
  label: Mailrith Email Templates API
  slug: mailrith-com-email-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-email-templates-api-openapi.yml
- filename: mailrith-com-forms-api-openapi.yml
  format: yaml
  label: Mailrith Forms API
  slug: mailrith-com-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-forms-api-openapi.yml
- filename: mailrith-com-jobs-api-openapi.yml
  format: yaml
  label: Mailrith Jobs API
  slug: mailrith-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-jobs-api-openapi.yml
- filename: mailrith-com-landing-pages-api-openapi.yml
  format: yaml
  label: Mailrith Landing Pages API
  slug: mailrith-com-landing-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-landing-pages-api-openapi.yml
- filename: mailrith-com-magic-links-api-openapi.yml
  format: yaml
  label: Mailrith Magic Links API
  slug: mailrith-com-magic-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-magic-links-api-openapi.yml
- filename: mailrith-com-platform-api-openapi.yml
  format: yaml
  label: Mailrith Platform API
  slug: mailrith-com-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-platform-api-openapi.yml
- filename: mailrith-com-segments-api-openapi.yml
  format: yaml
  label: Mailrith Segments API
  slug: mailrith-com-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-segments-api-openapi.yml
- filename: mailrith-com-sender-identities-api-openapi.yml
  format: yaml
  label: Mailrith Sender Identities API
  slug: mailrith-com-sender-identities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-sender-identities-api-openapi.yml
- filename: mailrith-com-sequences-api-openapi.yml
  format: yaml
  label: Mailrith Sequences API
  slug: mailrith-com-sequences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-sequences-api-openapi.yml
- filename: mailrith-com-starting-points-api-openapi.yml
  format: yaml
  label: Mailrith Starting Points API
  slug: mailrith-com-starting-points-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-starting-points-api-openapi.yml
- filename: mailrith-com-subscribers-api-openapi.yml
  format: yaml
  label: Mailrith Subscribers API
  slug: mailrith-com-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-subscribers-api-openapi.yml
- filename: mailrith-com-tags-api-openapi.yml
  format: yaml
  label: Mailrith Tags API
  slug: mailrith-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-tags-api-openapi.yml
- filename: mailrith-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: Mailrith Webhook Subscriptions API
  slug: mailrith-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-webhook-subscriptions-api-openapi.yml
- filename: mailrith-com-webhooks-api-openapi.yml
  format: yaml
  label: Mailrith Webhooks API
  slug: mailrith-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-webhooks-api-openapi.yml
- filename: mailrith-com-workspace-api-openapi.yml
  format: yaml
  label: Mailrith Workspace API
  slug: mailrith-com-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailrith-com/openapi/mailrith-com-workspace-api-openapi.yml
auth_types: []
description: Authentication schemes for Mailrith API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mailrith Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailrith declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Mailrith
provider_slug: mailrith-com
scheme_count: 2
schemes:
- evidence: Every protected `v1` request uses a Workspace API key or an authorized OAuth access token.
  header: Authorization
  how_to_obtain: Create a workspace API key in the Mailrith Settings → API Keys page.
  location: header
  name: Workspace API Key
  type: http-bearer
- authorize_url: https://api.mailrith.com/oauth/authorize
  evidence: Send the credential in the standard Authorization header.
  flows:
  - authorization_code
  - refresh_token
  header: Authorization
  how_to_obtain: Register an OAuth client at the registration_endpoint and follow the Authorization Code flow as described in the discovery document.
  location: header
  name: OAuth Access Token
  scopes:
  - analytics:read
  - live_actions:write
  - subscribers:read
  - subscribers:write
  - subscribers:import
  - subscribers:export
  - segments:read
  - segments:write
  - tags:read
  - tags:write
  - forms:read
  - forms:write
  - form_submissions:read
  - landing_pages:read
  - landing_pages:write
  - landing_page_submissions:read
  - broadcasts:read
  - broadcasts:write
  - sequences:read
  - sequences:write
  - magic_links:read
  - magic_links:write
  - automations:read
  - automations:write
  - workspace:read
  - email_templates:read
  - email_templates:write
  - custom_fields:read
  - custom_fields:write
  - webhooks:read
  - webhooks:write
  token_url: https://api.mailrith.com/oauth/token
  type: http-bearer
slug: mailrith-com-authentication
source_filename: mailrith-com-authentication.yml
source_heading: Authentication Profile
source_url: https://api.mailrith.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.mailrith.com/.well-known/oauth-authorization-server\nsources:\n- https://api.mailrith.com/.well-known/oauth-authorization-server\n- https://mailrith.com/developers/authentication\n- https://mailrith.com/developers/quickstart\n- https://mailrith.com/developers/zapier\ndescription: Authentication schemes for Mailrith API\nschemes:\n- type: http-bearer\n  name: Workspace API Key\n  evidence: Every protected `v1` request uses a Workspace API key or an authorized OAuth access token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a workspace API key in the Mailrith Settings → API Keys page.\n- type: http-bearer\n  name: OAuth Access Token\n  evidence: Send the credential in the standard Authorization header.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  - refresh_token\n  token_url: https://api.mailrith.com/oauth/token\n\
  \  authorize_url: https://api.mailrith.com/oauth/authorize\n  scopes:\n  - analytics:read\n  - live_actions:write\n  - subscribers:read\n  - subscribers:write\n  - subscribers:import\n  - subscribers:export\n  - segments:read\n  - segments:write\n  - tags:read\n  - tags:write\n  - forms:read\n  - forms:write\n  - form_submissions:read\n  - landing_pages:read\n  - landing_pages:write\n  - landing_page_submissions:read\n  - broadcasts:read\n  - broadcasts:write\n  - sequences:read\n  - sequences:write\n  - magic_links:read\n  - magic_links:write\n  - automations:read\n  - automations:write\n  - workspace:read\n  - email_templates:read\n  - email_templates:write\n  - custom_fields:read\n  - custom_fields:write\n  - webhooks:read\n  - webhooks:write\n  how_to_obtain: Register an OAuth client at the registration_endpoint and follow the Authorization Code flow as described in the discovery document.\ndocs: https://api.mailrith.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/mailrith-com/authentication/mailrith-com-authentication.yml
summary_line: 2 schemes
tags:
- Email Marketing
- Automation
- Software-as-a-Service
- Marketing
- Platform
---
