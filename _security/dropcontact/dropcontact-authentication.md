---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dropcontact-account-api-openapi.yml
  format: yaml
  label: Dropcontact Account API
  slug: dropcontact-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropcontact/openapi/dropcontact-account-api-openapi.yml
- filename: dropcontact-enrich-api-openapi.yml
  format: yaml
  label: Dropcontact Enrich API
  slug: dropcontact-enrich-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropcontact/openapi/dropcontact-enrich-api-openapi.yml
- filename: dropcontact-webhook-api-openapi.yml
  format: yaml
  label: Dropcontact Webhook API
  slug: dropcontact-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dropcontact/openapi/dropcontact-webhook-api-openapi.yml
auth_types: []
description: Authenticate the Dropcontact API with your API key
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dropcontact Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dropcontact declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Dropcontact
provider_slug: dropcontact
scheme_count: 1
schemes:
- evidence: The Dropcontact REST API uses an API key in the X-Access-Token request header.
  header: X-Access-Token
  how_to_obtain: Create and copy your API key in the Dropcontact app.
  location: header
  name: API Key
  type: apiKey
slug: dropcontact-authentication
source_filename: dropcontact-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.dropcontact.com/en/authentication/
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.dropcontact.com/en/authentication/\nsources:\n- https://developer.dropcontact.com/en/authentication/\n- https://developer.dropcontact.com/fr/authentication/\n- https://developer.dropcontact.com/en/authentication/\n- https://developer.dropcontact.com/en/quickstart/\ndescription: Authenticate the Dropcontact API with your API key\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: The Dropcontact REST API uses an API key in the X-Access-Token request header.\n  location: header\n  header: X-Access-Token\n  how_to_obtain: Create and copy your API key in the Dropcontact app.\ndocs: https://developer.dropcontact.com/en/authentication/\n"
source_yaml_url: https://artifacts.apis.io/dropcontact/authentication/dropcontact-authentication.yml
summary_line: 1 scheme
tags:
- B2B
- Email Finder
- Data Enrichment
- GDPR
- CRM Integration
---
