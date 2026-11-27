---
anonymous_access: false
api_key_in: []
api_specs:
- filename: richpanel-channel-api-openapi.yml
  format: yaml
  label: Richpanel Channel API
  slug: richpanel-channel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/richpanel/openapi/richpanel-channel-api-openapi.yml
- filename: richpanel-customers-api-openapi.yml
  format: yaml
  label: Richpanel Customers API
  slug: richpanel-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/richpanel/openapi/richpanel-customers-api-openapi.yml
- filename: richpanel-file-api-openapi.yml
  format: yaml
  label: Richpanel File API
  slug: richpanel-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/richpanel/openapi/richpanel-file-api-openapi.yml
- filename: richpanel-order-api-openapi.yml
  format: yaml
  label: Richpanel Order API
  slug: richpanel-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/richpanel/openapi/richpanel-order-api-openapi.yml
- filename: richpanel-reports-api-openapi.yml
  format: yaml
  label: Richpanel Reports API
  slug: richpanel-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/richpanel/openapi/richpanel-reports-api-openapi.yml
- filename: richpanel-subscription-api-openapi.yml
  format: yaml
  label: Richpanel Subscription API
  slug: richpanel-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/richpanel/openapi/richpanel-subscription-api-openapi.yml
- filename: richpanel-tags-api-openapi.yml
  format: yaml
  label: Richpanel Tags API
  slug: richpanel-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/richpanel/openapi/richpanel-tags-api-openapi.yml
- filename: richpanel-tasks-api-openapi.yml
  format: yaml
  label: Richpanel Tasks API
  slug: richpanel-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/richpanel/openapi/richpanel-tasks-api-openapi.yml
- filename: richpanel-teams-api-openapi.yml
  format: yaml
  label: Richpanel Teams API
  slug: richpanel-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/richpanel/openapi/richpanel-teams-api-openapi.yml
- filename: richpanel-tickets-api-openapi.yml
  format: yaml
  label: Richpanel Tickets API
  slug: richpanel-tickets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/richpanel/openapi/richpanel-tickets-api-openapi.yml
- filename: richpanel-users-api-openapi.yml
  format: yaml
  label: Richpanel Users API
  slug: richpanel-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/richpanel/openapi/richpanel-users-api-openapi.yml
auth_types: []
description: Richpanel provides API key authentication for both the Helpdesk API and the Returns API.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Richpanel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Richpanel declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Richpanel
provider_slug: richpanel
scheme_count: 2
schemes:
- evidence: You need to pass this API Key in your request header with **x-richpanel-key**.
  header: x-richpanel-key
  how_to_obtain: View or generate an API key in your Richpanel account under Settings → Integrations → API Keys.
  location: header
  name: Helpdesk API Key
  type: apiKey
- evidence: All requests require an `x-api-key` header.
  header: x-api-key
  how_to_obtain: Generate a dedicated Returns API key via Returns Dashboard → Settings → API Keys.
  location: header
  name: Returns API Key
  scopes:
  - RETURNS
  - SETTINGS
  - REASON
  - CUSTOMIZATION
  - ANALYTIC
  - CUSTOMER_EXPERIENCE
  type: apiKey
slug: richpanel-authentication
source_filename: richpanel-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.richpanel.com/reference/authentication.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.richpanel.com/reference/authentication.md\nsources:\n- https://developer.richpanel.com/reference/authentication.md\n- https://developer.richpanel.com/reference/returns-api-auth.md\n- https://developer.richpanel.com/reference/authentication\n- https://developer.richpanel.com/reference/returns-api-auth\ndescription: Richpanel provides API key authentication for both the Helpdesk API and the Returns API.\nschemes:\n- type: apiKey\n  name: Helpdesk API Key\n  evidence: You need to pass this API Key in your request header with **x-richpanel-key**.\n  location: header\n  header: x-richpanel-key\n  how_to_obtain: View or generate an API key in your Richpanel account under Settings → Integrations → API Keys.\n- type: apiKey\n  name: Returns API Key\n  evidence: All requests require an `x-api-key` header.\n  location: header\n  header: x-api-key\n  scopes:\n  - RETURNS\n\
  \  - SETTINGS\n  - REASON\n  - CUSTOMIZATION\n  - ANALYTIC\n  - CUSTOMER_EXPERIENCE\n  how_to_obtain: Generate a dedicated Returns API key via Returns Dashboard → Settings → API Keys.\ndocs: https://developer.richpanel.com/reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/richpanel/authentication/richpanel-authentication.yml
summary_line: 2 schemes
tags:
- Help Desk
- AI Support
- E-Commerce
- Automation
---
