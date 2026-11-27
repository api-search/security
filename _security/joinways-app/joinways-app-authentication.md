---
anonymous_access: false
api_key_in: []
api_specs:
- filename: joinways-app-analytics-api-openapi.yml
  format: yaml
  label: Joinways Analytics API
  slug: joinways-app-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-analytics-api-openapi.yml
- filename: joinways-app-catalog-api-openapi.yml
  format: yaml
  label: Joinways Catalog API
  slug: joinways-app-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-catalog-api-openapi.yml
- filename: joinways-app-companies-api-openapi.yml
  format: yaml
  label: Joinways Companies API
  slug: joinways-app-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-companies-api-openapi.yml
- filename: joinways-app-events-api-openapi.yml
  format: yaml
  label: Joinways Events API
  slug: joinways-app-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-events-api-openapi.yml
- filename: joinways-app-invoices-api-openapi.yml
  format: yaml
  label: Joinways Invoices API
  slug: joinways-app-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-invoices-api-openapi.yml
- filename: joinways-app-leads-api-openapi.yml
  format: yaml
  label: Joinways Leads API
  slug: joinways-app-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-leads-api-openapi.yml
- filename: joinways-app-notifications-api-openapi.yml
  format: yaml
  label: Joinways Notifications API
  slug: joinways-app-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-notifications-api-openapi.yml
- filename: joinways-app-people-api-openapi.yml
  format: yaml
  label: Joinways People API
  slug: joinways-app-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-people-api-openapi.yml
- filename: joinways-app-quotes-api-openapi.yml
  format: yaml
  label: Joinways Quotes API
  slug: joinways-app-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-quotes-api-openapi.yml
- filename: joinways-app-search-api-openapi.yml
  format: yaml
  label: Joinways Search API
  slug: joinways-app-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-search-api-openapi.yml
- filename: joinways-app-tasks-api-openapi.yml
  format: yaml
  label: Joinways Tasks API
  slug: joinways-app-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-tasks-api-openapi.yml
- filename: joinways-app-team-api-openapi.yml
  format: yaml
  label: Joinways Team API
  slug: joinways-app-team-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-team-api-openapi.yml
- filename: joinways-app-venues-api-openapi.yml
  format: yaml
  label: Joinways Venues API
  slug: joinways-app-venues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-venues-api-openapi.yml
- filename: joinways-app-webhooks-api-openapi.yml
  format: yaml
  label: Joinways Webhooks API
  slug: joinways-app-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinways-app/openapi/joinways-app-webhooks-api-openapi.yml
auth_types: []
description: Joinways authenticates API requests using an API key passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Joinways Authentication
name_suffix: Authentication
oauth_flows: []
overview: Joinways declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Joinways
provider_slug: joinways-app
scheme_count: 1
schemes:
- evidence: Add the key in the Authorization header, as Bearer jw_…
  header: Authorization
  how_to_obtain: Create an API key in Settings > Developers, copy the key (prefix jw_…) and use it as a Bearer token.
  location: header
  name: API Key
  type: http-bearer
slug: joinways-app-authentication
source_filename: joinways-app-authentication.yml
source_heading: Authentication Profile
source_url: https://joinways.app/docs/category/tools
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://joinways.app/docs/category/tools\nsources:\n- https://joinways.app/docs/category/tools\n- https://joinways.app/docs/api-keys\n- https://joinways.app/blog/onboarding-new-events-salesperson-knowledge-transfer\n- https://joinways.app/blog/hiring-venue-sales-manager-2026-profile-package-onboarding\ndescription: Joinways authenticates API requests using an API key passed as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Add the key in the Authorization header, as Bearer jw_…\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings > Developers, copy the key (prefix jw_…) and use it as a Bearer token.\nnote: No other authentication schemes (apiKey, oauth2, http-basic, jwt, hmac, mtls, other) are documented.\ndocs: https://joinways.app/docs/category/tools\n"
source_yaml_url: https://artifacts.apis.io/joinways-app/authentication/joinways-app-authentication.yml
summary_line: 1 scheme
tags:
- Event Management
- Software-as-a-Service
- CRM
- Venue Software
- Multilingual
---
