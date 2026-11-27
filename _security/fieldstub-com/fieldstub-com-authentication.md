---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fieldstub-com-links-api-openapi.yml
  format: yaml
  label: Fieldstub Links API
  slug: fieldstub-com-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fieldstub-com/openapi/fieldstub-com-links-api-openapi.yml
- filename: fieldstub-com-projects-api-openapi.yml
  format: yaml
  label: Fieldstub Projects API
  slug: fieldstub-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fieldstub-com/openapi/fieldstub-com-projects-api-openapi.yml
- filename: fieldstub-com-tickets-api-openapi.yml
  format: yaml
  label: Fieldstub Tickets API
  slug: fieldstub-com-tickets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fieldstub-com/openapi/fieldstub-com-tickets-api-openapi.yml
auth_types: []
description: 'Auth: a service account, not per-user OAuth'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fieldstub Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fieldstub declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fieldstub
provider_slug: fieldstub-com
scheme_count: 1
schemes:
- evidence: 'Auth: a service account, not per-user OAuth'
  flows:
  - client_credentials
  how_to_obtain: A Data Management Service Account (DMSA) with client_credentials works for reads and writes
  name: Procore Service Account
  token_url: https://login.procore.com/oauth/token
  type: oauth2
slug: fieldstub-com-authentication
source_filename: fieldstub-com-authentication.yml
source_heading: Authentication Profile
source_url: https://fieldstub.com/docs/procore-change-events-api
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fieldstub.com/docs/procore-change-events-api\nsources:\n- https://fieldstub.com/docs/procore-change-events-api\ndescription: 'Auth: a service account, not per-user OAuth'\nschemes:\n- type: oauth2\n  name: Procore Service Account\n  evidence: 'Auth: a service account, not per-user OAuth'\n  flows:\n  - client_credentials\n  token_url: https://login.procore.com/oauth/token\n  how_to_obtain: A Data Management Service Account (DMSA) with client_credentials works for reads and writes\ndocs: https://fieldstub.com/docs/procore-change-events-api\n"
source_yaml_url: https://artifacts.apis.io/fieldstub-com/authentication/fieldstub-com-authentication.yml
summary_line: 1 scheme
tags:
- Construction
- Field Service Management
- Procore Integration
- Time and Materials
- NoLogin
---
