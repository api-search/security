---
anonymous_access: false
api_key_in: []
api_specs:
- filename: text-in-church-account-api-openapi.yml
  format: yaml
  label: Text In Church Account API
  slug: text-in-church-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-account-api-openapi.yml
- filename: text-in-church-billing-api-openapi.yml
  format: yaml
  label: Text In Church Billing API
  slug: text-in-church-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-billing-api-openapi.yml
- filename: text-in-church-calling-api-openapi.yml
  format: yaml
  label: Text In Church Calling API
  slug: text-in-church-calling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-calling-api-openapi.yml
- filename: text-in-church-connect-cards-api-openapi.yml
  format: yaml
  label: Text In Church Connect Cards API
  slug: text-in-church-connect-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-connect-cards-api-openapi.yml
- filename: text-in-church-data-capture-api-openapi.yml
  format: yaml
  label: Text In Church Data Capture API
  slug: text-in-church-data-capture-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-data-capture-api-openapi.yml
- filename: text-in-church-enum-api-openapi.yml
  format: yaml
  label: Text In Church Enum API
  slug: text-in-church-enum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-enum-api-openapi.yml
- filename: text-in-church-groups-api-openapi.yml
  format: yaml
  label: Text In Church Groups API
  slug: text-in-church-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-groups-api-openapi.yml
- filename: text-in-church-integrations-api-openapi.yml
  format: yaml
  label: Text In Church Integrations API
  slug: text-in-church-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-integrations-api-openapi.yml
- filename: text-in-church-messaging-api-openapi.yml
  format: yaml
  label: Text In Church Messaging API
  slug: text-in-church-messaging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-messaging-api-openapi.yml
- filename: text-in-church-pages-api-openapi.yml
  format: yaml
  label: Text In Church Pages API
  slug: text-in-church-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-pages-api-openapi.yml
- filename: text-in-church-people-api-openapi.yml
  format: yaml
  label: Text In Church People API
  slug: text-in-church-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-people-api-openapi.yml
- filename: text-in-church-phone-numbers-api-openapi.yml
  format: yaml
  label: Text In Church Phone Numbers API
  slug: text-in-church-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-phone-numbers-api-openapi.yml
- filename: text-in-church-tasks-api-openapi.yml
  format: yaml
  label: Text In Church Tasks API
  slug: text-in-church-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-tasks-api-openapi.yml
- filename: text-in-church-tools-api-openapi.yml
  format: yaml
  label: Text In Church Tools API
  slug: text-in-church-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-tools-api-openapi.yml
- filename: text-in-church-users-api-openapi.yml
  format: yaml
  label: Text In Church Users API
  slug: text-in-church-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-users-api-openapi.yml
- filename: text-in-church-webhooks-api-openapi.yml
  format: yaml
  label: Text In Church Webhooks API
  slug: text-in-church-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-webhooks-api-openapi.yml
- filename: text-in-church-workflows-api-openapi.yml
  format: yaml
  label: Text In Church Workflows API
  slug: text-in-church-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/text-in-church/openapi/text-in-church-workflows-api-openapi.yml
auth_types: []
description: Authentication methods for Text In Church API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Text In Church Authentication
name_suffix: Authentication
oauth_flows: []
overview: Text In Church declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Text In Church
provider_slug: text-in-church
scheme_count: 2
schemes:
- evidence: To use the API Key, just pass it to the API in the header of your request as the authorization bearer token.
  header: authorization
  how_to_obtain: Create an API key in the Text In Church account under Account Settings → Developer API.
  location: header
  name: Personal API Key
  type: http-bearer
- authorize_url: https://api.textinchurch.com/API/1_0/oauthorize.php?client_id=CLIENT_ID&redirect_uri=https://your-application/callback&response_type=code
  evidence: Text In Church conforms to the Authorization Code flow in OAuth version 2.0.
  how_to_obtain: Create an OAuth application in the developer area after contacting support for access.
  name: OAuth 2.0
  scopes:
  - people
  token_url: https://api.textinchurch.com/API/1_0/oauthorize.php
  type: oauth2
slug: text-in-church-authentication
source_filename: text-in-church-authentication.yml
source_heading: Authentication Profile
source_url: https://api-docs.textinchurch.com/docs/authentication.md
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api-docs.textinchurch.com/docs/authentication.md\nsources:\n- https://api-docs.textinchurch.com/docs/authentication.md\n- https://api-docs.textinchurch.com/docs/authentication\n- https://api-docs.textinchurch.com/docs/getting-started.md\n- https://api-docs.textinchurch.com/docs/getting-started\ndescription: Authentication methods for Text In Church API\nschemes:\n- type: http-bearer\n  name: Personal API Key\n  evidence: To use the API Key, just pass it to the API in the header of your request as the authorization bearer token.\n  location: header\n  header: authorization\n  how_to_obtain: Create an API key in the Text In Church account under Account Settings → Developer API.\n- type: oauth2\n  name: OAuth 2.0\n  evidence: Text In Church conforms to the Authorization Code flow in OAuth version 2.0.\n  token_url: https://api.textinchurch.com/API/1_0/oauthorize.php\n  authorize_url:\
  \ https://api.textinchurch.com/API/1_0/oauthorize.php?client_id=CLIENT_ID&redirect_uri=https://your-application/callback&response_type=code\n  scopes:\n  - people\n  how_to_obtain: Create an OAuth application in the developer area after contacting support for access.\ndocs: https://api-docs.textinchurch.com/docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/text-in-church/authentication/text-in-church-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Communications
- Church
- Messaging
- Automation
---
