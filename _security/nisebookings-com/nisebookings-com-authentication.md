---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nisebookings-com-availability-api-openapi.yml
  format: yaml
  label: nisebookings Availability API
  slug: nisebookings-com-availability-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nisebookings-com/openapi/nisebookings-com-availability-api-openapi.yml
- filename: nisebookings-com-bookings-api-openapi.yml
  format: yaml
  label: nisebookings Bookings API
  slug: nisebookings-com-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nisebookings-com/openapi/nisebookings-com-bookings-api-openapi.yml
- filename: nisebookings-com-catalogue-api-openapi.yml
  format: yaml
  label: nisebookings Catalogue API
  slug: nisebookings-com-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nisebookings-com/openapi/nisebookings-com-catalogue-api-openapi.yml
- filename: nisebookings-com-events-api-openapi.yml
  format: yaml
  label: nisebookings Events API
  slug: nisebookings-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nisebookings-com/openapi/nisebookings-com-events-api-openapi.yml
- filename: nisebookings-com-packages-api-openapi.yml
  format: yaml
  label: nisebookings Packages API
  slug: nisebookings-com-packages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nisebookings-com/openapi/nisebookings-com-packages-api-openapi.yml
- filename: nisebookings-com-payments-api-openapi.yml
  format: yaml
  label: nisebookings Payments API
  slug: nisebookings-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nisebookings-com/openapi/nisebookings-com-payments-api-openapi.yml
- filename: nisebookings-com-sandbox-api-openapi.yml
  format: yaml
  label: nisebookings Sandbox API
  slug: nisebookings-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nisebookings-com/openapi/nisebookings-com-sandbox-api-openapi.yml
auth_types: []
description: Authentication uses a Bearer token passed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: nisebookings Authentication
name_suffix: Authentication
oauth_flows: []
overview: nisebookings declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: nisebookings
provider_slug: nisebookings-com
scheme_count: 1
schemes:
- evidence: 'curl -s -H "Authorization: Bearer $KEY" $API/me'
  header: Authorization
  how_to_obtain: Create an account, go to Settings → API and generate a key (e.g., nk_…).
  location: header
  name: Bearer
  type: http-bearer
slug: nisebookings-com-authentication
source_filename: nisebookings-com-authentication.yml
source_heading: Authentication Profile
source_url: https://guide.nisebookings.com/01-quickstart.html
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://guide.nisebookings.com/01-quickstart.html\nsources:\n- https://guide.nisebookings.com/01-quickstart.html\ndescription: Authentication uses a Bearer token passed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl -s -H \"Authorization: Bearer $KEY\" $API/me'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an account, go to Settings → API and generate a key (e.g., nk_…).\ndocs: https://guide.nisebookings.com/01-quickstart.html\n"
source_yaml_url: https://artifacts.apis.io/nisebookings-com/authentication/nisebookings-com-authentication.yml
summary_line: 1 scheme
tags:
- Booking
- Software-as-a-Service
- Scheduling
- Payments
---
