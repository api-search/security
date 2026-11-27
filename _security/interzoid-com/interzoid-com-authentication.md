---
anonymous_access: false
api_key_in: []
api_specs:
- filename: interzoid-com-data-enhancement-api-openapi.yml
  format: yaml
  label: Interzoid Data Enhancement API
  slug: interzoid-com-data-enhancement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/interzoid-com/openapi/interzoid-com-data-enhancement-api-openapi.yml
- filename: interzoid-com-data-enrichment-api-openapi.yml
  format: yaml
  label: Interzoid Data Enrichment API
  slug: interzoid-com-data-enrichment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/interzoid-com/openapi/interzoid-com-data-enrichment-api-openapi.yml
- filename: interzoid-com-data-matching-api-openapi.yml
  format: yaml
  label: Interzoid Data Matching API
  slug: interzoid-com-data-matching-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/interzoid-com/openapi/interzoid-com-data-matching-api-openapi.yml
- filename: interzoid-com-data-standardization-api-openapi.yml
  format: yaml
  label: Interzoid Data Standardization API
  slug: interzoid-com-data-standardization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/interzoid-com/openapi/interzoid-com-data-standardization-api-openapi.yml
- filename: interzoid-com-utility-api-openapi.yml
  format: yaml
  label: Interzoid Utility API
  slug: interzoid-com-utility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/interzoid-com/openapi/interzoid-com-utility-api-openapi.yml
auth_types: []
description: Interzoid uses an API license key for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Interzoid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Interzoid declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Interzoid
provider_slug: interzoid-com
scheme_count: 1
schemes:
- evidence: After registration, log in to your account and navigate to the "Account" section where you will find your unique API license key. You will use this to authenticate your requests to Interzoid tools, products, and APIs.
  how_to_obtain: Obtain from the Account section after creating an Interzoid account.
  location: query
  name: API Key
  type: apiKey
slug: interzoid-com-authentication
source_filename: interzoid-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.interzoid.com/entries/getting-started
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.interzoid.com/entries/getting-started\nsources:\n- https://docs.interzoid.com/entries/getting-started\ndescription: Interzoid uses an API license key for authentication.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: After registration, log in to your account and navigate to the \"Account\" section where you will find your unique API license key.\n    You will use this to authenticate your requests to Interzoid tools, products, and APIs.\n  location: query\n  how_to_obtain: Obtain from the Account section after creating an Interzoid account.\ndocs: https://docs.interzoid.com/entries/getting-started\n"
source_yaml_url: https://artifacts.apis.io/interzoid-com/authentication/interzoid-com-authentication.yml
summary_line: 1 scheme
tags:
- Data
- Data Enrichment
- Matching
- Business Intelligence
---
