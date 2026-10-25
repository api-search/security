---
anonymous_access: false
api_key_in: []
api_specs:
- filename: public-transport-victoria-departures-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Departures API
  slug: public-transport-victoria-departures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-departures-api-openapi.yml
- filename: public-transport-victoria-directions-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Directions API
  slug: public-transport-victoria-directions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-directions-api-openapi.yml
- filename: public-transport-victoria-disruptions-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Disruptions API
  slug: public-transport-victoria-disruptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-disruptions-api-openapi.yml
- filename: public-transport-victoria-fareestimate-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Fare Estimate API
  slug: public-transport-victoria-fareestimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-fareestimate-api-openapi.yml
- filename: public-transport-victoria-outlets-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Outlets API
  slug: public-transport-victoria-outlets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-outlets-api-openapi.yml
- filename: public-transport-victoria-patterns-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Patterns API
  slug: public-transport-victoria-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-patterns-api-openapi.yml
- filename: public-transport-victoria-routes-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Routes API
  slug: public-transport-victoria-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-routes-api-openapi.yml
- filename: public-transport-victoria-routetypes-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Route Types API
  slug: public-transport-victoria-routetypes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-routetypes-api-openapi.yml
- filename: public-transport-victoria-runs-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Runs API
  slug: public-transport-victoria-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-runs-api-openapi.yml
- filename: public-transport-victoria-search-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Search API
  slug: public-transport-victoria-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-search-api-openapi.yml
- filename: public-transport-victoria-stops-api-openapi.yml
  format: yaml
  label: Public Transport Victoria Stops API
  slug: public-transport-victoria-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/openapi/public-transport-victoria-stops-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Public Transport Victoria Authentication
name_suffix: Authentication
oauth_flows: []
overview: Public Transport Victoria declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Public Transport Victoria
provider_slug: public-transport-victoria
scheme_count: 1
schemes:
- algorithm: HMAC-SHA1
  case_sensitive: true
  in: query
  key_expiry: If you haven't used the API for over 3 months, we may disable your API key and remove you from the list – but you can always register for a new key if you need one.
  key_format: The API key consists of a 128bit GUID.
  name: devid-hmac-signature
  parameters:
  - description: User Id ("devid") issued by PTV
    name: devid
  - description: HMAC-SHA1 of the request path and query (minus the base URL, including devid), keyed with the API key
    name: signature
  provisioning:
    self_service: false
    text: Send an email to APIKeyRequest@ptv.vic.gov.au with "PTV Timetable API – request for key" in the subject line; PTV sends an API key and a user Id by return email.
  samples:
  - C#
  - Java
  - Objective C
  - Python
  signature_text: The signature value is a HMAC-SHA1 hash of the completed request (minus the base URL but including your user ID, known as "devid") and the API key
  type: apiKey
slug: public-transport-victoria-authentication
source_filename: public-transport-victoria-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: searched\nsource: https://www.vic.gov.au/sites/default/files/2025-06/PTV-Timetable-API-key-and-signature-document.rtf\ndocs: https://www.vic.gov.au/public-transport-timetable-api\nnote: The Swagger 2.0 contract declares no securityDefinitions; every operation instead takes `devid` (\"Your developer id\") and `signature` (\"Authentication signature for request\") query parameters. Scheme details below are from PTV's key-and-signature document.\nschemes:\n- name: devid-hmac-signature\n  type: apiKey\n  in: query\n  parameters:\n  - name: devid\n    description: User Id (\"devid\") issued by PTV\n  - name: signature\n    description: HMAC-SHA1 of the request path and query (minus the base URL, including devid), keyed with the API key\n  algorithm: HMAC-SHA1\n  key_format: The API key consists of a 128bit GUID.\n  signature_text: 'The signature value is a HMAC-SHA1 hash of the completed request (minus the base URL but including your user ID, known\
  \ as \"devid\") and the API key'\n  case_sensitive: true\n  provisioning:\n    self_service: false\n    text: Send an email to APIKeyRequest@ptv.vic.gov.au with \"PTV Timetable API – request for key\" in the subject line; PTV sends an API key and a user Id by return email.\n  key_expiry: If you haven't used the API for over 3 months, we may disable your API key and remove you from the list – but you can always register for a new key if you need one.\n  samples: [C#, Java, Objective C, Python]\noauth: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/public-transport-victoria/refs/heads/main/authentication/public-transport-victoria-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Public Transport
- Government
- Transit
- Timetables
- Australia
- Open Data
---
