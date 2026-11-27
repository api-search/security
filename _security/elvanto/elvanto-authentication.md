---
anonymous_access: false
api_key_in: []
api_specs:
- filename: elvanto-accounts-api-openapi.yml
  format: yaml
  label: Elvanto Accounts API
  slug: elvanto-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elvanto/openapi/elvanto-accounts-api-openapi.yml
- filename: elvanto-accounts-list-all-api-openapi.yml
  format: yaml
  label: Elvanto Accounts List All API
  slug: elvanto-accounts-list-all-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elvanto/openapi/elvanto-accounts-list-all-api-openapi.yml
- filename: elvanto-accounts-list-api-openapi.yml
  format: yaml
  label: Elvanto Accounts List API
  slug: elvanto-accounts-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elvanto/openapi/elvanto-accounts-list-api-openapi.yml
- filename: elvanto-charge-once-api-openapi.yml
  format: yaml
  label: Elvanto Charge Once API
  slug: elvanto-charge-once-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elvanto/openapi/elvanto-charge-once-api-openapi.yml
- filename: elvanto-charges-api-openapi.yml
  format: yaml
  label: Elvanto Charges API
  slug: elvanto-charges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elvanto/openapi/elvanto-charges-api-openapi.yml
- filename: elvanto-charges-list-api-openapi.yml
  format: yaml
  label: Elvanto Charges List API
  slug: elvanto-charges-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elvanto/openapi/elvanto-charges-list-api-openapi.yml
- filename: elvanto-organizations-api-openapi.yml
  format: yaml
  label: Elvanto Organizations API
  slug: elvanto-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elvanto/openapi/elvanto-organizations-api-openapi.yml
- filename: elvanto-organizations-list-api-openapi.yml
  format: yaml
  label: Elvanto Organizations List API
  slug: elvanto-organizations-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elvanto/openapi/elvanto-organizations-list-api-openapi.yml
- filename: elvanto-payment-methods-api-openapi.yml
  format: yaml
  label: Elvanto Payment Methods API
  slug: elvanto-payment-methods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elvanto/openapi/elvanto-payment-methods-api-openapi.yml
- filename: elvanto-payment-methods-list-api-openapi.yml
  format: yaml
  label: Elvanto Payment Methods List API
  slug: elvanto-payment-methods-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elvanto/openapi/elvanto-payment-methods-list-api-openapi.yml
- filename: elvanto-recurring-api-openapi.yml
  format: yaml
  label: Elvanto Recurring API
  slug: elvanto-recurring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elvanto/openapi/elvanto-recurring-api-openapi.yml
- filename: elvanto-recurring-list-api-openapi.yml
  format: yaml
  label: Elvanto Recurring List API
  slug: elvanto-recurring-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elvanto/openapi/elvanto-recurring-list-api-openapi.yml
- filename: elvanto-refunds-api-openapi.yml
  format: yaml
  label: Elvanto Refunds API
  slug: elvanto-refunds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/elvanto/openapi/elvanto-refunds-api-openapi.yml
auth_types: []
description: Elvanto API authentication methods
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Elvanto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elvanto declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Elvanto
provider_slug: elvanto
scheme_count: 2
schemes:
- authorize_url: https://api.elvanto.com/oauth?type=web_server&client_id={client_id}&redirect_uri={redirect_uri}&scope={scope}&state={state}
  evidence: The Elvanto API currently supports two methods of authentication. We recommend authenticating with OAuth, however we also support authenticating with an API key.
  flows:
  - authorization_code
  - implicit
  how_to_obtain: Register an OAuth Application in your Elvanto account settings under Integrations to receive a Client ID and Client Secret.
  name: OAuth 2
  scopes:
  - ManagePeople
  - ManageGroups
  - ManageServices
  - ManageSongs
  - ManageCalendar
  - ManageFinancials
  - AdministerAccount
  type: oauth2
- evidence: The Elvanto API currently supports two methods of authentication. We recommend authenticating with OAuth, however we also support authenticating with an API key.
  how_to_obtain: Create an API key in your Elvanto account settings (details not specified on the page).
  name: API Key
  type: apiKey
slug: elvanto-authentication
source_filename: elvanto-authentication.yml
source_heading: Authentication Profile
source_url: https://www.elvanto.com/api/people/currentUser
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.elvanto.com/api/people/currentUser\nsources:\n- https://www.elvanto.com/api/people/currentUser\n- https://www.elvanto.com/api/getting-started\n- https://docs.tithe.ly/reference/setup\ndescription: Elvanto API authentication methods\nschemes:\n- type: oauth2\n  name: OAuth 2\n  evidence: The Elvanto API currently supports two methods of authentication. We recommend authenticating with OAuth, however we also support\n    authenticating with an API key.\n  flows:\n  - authorization_code\n  - implicit\n  authorize_url: https://api.elvanto.com/oauth?type=web_server&client_id={client_id}&redirect_uri={redirect_uri}&scope={scope}&state={state}\n  scopes:\n  - ManagePeople\n  - ManageGroups\n  - ManageServices\n  - ManageSongs\n  - ManageCalendar\n  - ManageFinancials\n  - AdministerAccount\n  how_to_obtain: Register an OAuth Application in your Elvanto account settings under\
  \ Integrations to receive a Client ID and Client Secret.\n- type: apiKey\n  name: API Key\n  evidence: The Elvanto API currently supports two methods of authentication. We recommend authenticating with OAuth, however we also support\n    authenticating with an API key.\n  how_to_obtain: Create an API key in your Elvanto account settings (details not specified on the page).\ndocs: https://www.elvanto.com/api/people/currentUser\n"
source_yaml_url: https://artifacts.apis.io/elvanto/authentication/elvanto-authentication.yml
summary_line: 2 schemes
tags:
- Church Management
- Software
- Software-as-a-Service
- Cloud
- Non-Profit
---
