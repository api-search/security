---
anonymous_access: false
api_key_in: []
api_specs:
- filename: databazaar-io-account-api-openapi.yml
  format: yaml
  label: DataBazaar Account API
  slug: databazaar-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databazaar-io/openapi/databazaar-io-account-api-openapi.yml
- filename: databazaar-io-agent-api-openapi.yml
  format: yaml
  label: DataBazaar Agent API
  slug: databazaar-io-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databazaar-io/openapi/databazaar-io-agent-api-openapi.yml
- filename: databazaar-io-bounty-submissions-api-openapi.yml
  format: yaml
  label: DataBazaar Bounty Submissions API
  slug: databazaar-io-bounty-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databazaar-io/openapi/databazaar-io-bounty-submissions-api-openapi.yml
- filename: databazaar-io-categories-api-openapi.yml
  format: yaml
  label: DataBazaar Categories API
  slug: databazaar-io-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databazaar-io/openapi/databazaar-io-categories-api-openapi.yml
- filename: databazaar-io-datasets-api-openapi.yml
  format: yaml
  label: DataBazaar Datasets API
  slug: databazaar-io-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databazaar-io/openapi/databazaar-io-datasets-api-openapi.yml
- filename: databazaar-io-listings-api-openapi.yml
  format: yaml
  label: DataBazaar Listings API
  slug: databazaar-io-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databazaar-io/openapi/databazaar-io-listings-api-openapi.yml
- filename: databazaar-io-purchases-api-openapi.yml
  format: yaml
  label: DataBazaar Purchases API
  slug: databazaar-io-purchases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/databazaar-io/openapi/databazaar-io-purchases-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Databazaar Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataBazaar secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DataBazaar
provider_slug: databazaar-io
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/databazaar-io-openapi-full.yml
  - openapi/databazaar-io-openapi.yml
  type: http
slug: databazaar-io-authentication
source_filename: databazaar-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/databazaar-io-openapi-full.yml, openapi/databazaar-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/databazaar-io-openapi-full.yml\n  - openapi/databazaar-io-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/databazaar-io/authentication/databazaar-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Marketplace
- AI Agents
- Datasets
- Marketplace
- Agent-Native
---
