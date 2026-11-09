---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dataquoll-io-addresses-api-openapi.yml
  format: yaml
  label: DataQuoll Addresses API
  slug: dataquoll-io-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-addresses-api-openapi.yml
- filename: dataquoll-io-calendars-api-openapi.yml
  format: yaml
  label: DataQuoll Calendars API
  slug: dataquoll-io-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-calendars-api-openapi.yml
- filename: dataquoll-io-declarations-api-openapi.yml
  format: yaml
  label: DataQuoll Declarations API
  slug: dataquoll-io-declarations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-declarations-api-openapi.yml
- filename: dataquoll-io-events-api-openapi.yml
  format: yaml
  label: DataQuoll Events API
  slug: dataquoll-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-events-api-openapi.yml
- filename: dataquoll-io-facilities-api-openapi.yml
  format: yaml
  label: DataQuoll Facilities API
  slug: dataquoll-io-facilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-facilities-api-openapi.yml
- filename: dataquoll-io-gauges-api-openapi.yml
  format: yaml
  label: DataQuoll Gauges API
  slug: dataquoll-io-gauges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-gauges-api-openapi.yml
- filename: dataquoll-io-hazard-history-api-openapi.yml
  format: yaml
  label: DataQuoll Hazard history API
  slug: dataquoll-io-hazard-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-hazard-history-api-openapi.yml
- filename: dataquoll-io-incidents-api-openapi.yml
  format: yaml
  label: DataQuoll Incidents API
  slug: dataquoll-io-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-incidents-api-openapi.yml
- filename: dataquoll-io-meta-api-openapi.yml
  format: yaml
  label: DataQuoll Meta API
  slug: dataquoll-io-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-meta-api-openapi.yml
- filename: dataquoll-io-mobile-sites-api-openapi.yml
  format: yaml
  label: DataQuoll Mobile sites API
  slug: dataquoll-io-mobile-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-mobile-sites-api-openapi.yml
- filename: dataquoll-io-publications-api-openapi.yml
  format: yaml
  label: DataQuoll Publications API
  slug: dataquoll-io-publications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dataquoll-io/openapi/dataquoll-io-publications-api-openapi.yml
auth_types: []
description: DataQuoll uses an API key that is sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Dataquoll Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataQuoll declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DataQuoll
provider_slug: dataquoll-io
scheme_count: 1
schemes:
- evidence: 'curl -s "https://dataquoll.io/api/v1/incidents?limit=1" \ -H "Authorization: Bearer YOUR_API_KEY"'
  header: Authorization
  how_to_obtain: Sign up for a free account and grab your API key from the dashboard.
  location: header
  name: Authorization
  type: http-bearer
slug: dataquoll-io-authentication
source_filename: dataquoll-io-authentication.yml
source_heading: Authentication Profile
source_url: https://dataquoll.io/quickstart
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dataquoll.io/quickstart\nsources:\n- https://dataquoll.io/quickstart\n- https://dataquoll.io/guides/python-quickstart.md\ndescription: DataQuoll uses an API key that is sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'curl -s \"https://dataquoll.io/api/v1/incidents?limit=1\" \\ -H \"Authorization: Bearer YOUR_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up for a free account and grab your API key from the dashboard.\ndocs: https://dataquoll.io/quickstart\n"
source_yaml_url: https://artifacts.apis.io/dataquoll-io/authentication/dataquoll-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data
- Emergency
- Australia
- Public Data
---
