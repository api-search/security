---
anonymous_access: false
api_key_in: []
api_specs:
- filename: twitterapi-io-oapi-api-openapi.yml
  format: yaml
  label: TwitterAPI.io Oapi API
  slug: twitterapi-io-oapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitterapi-io/openapi/twitterapi-io-oapi-api-openapi.yml
- filename: twitterapi-io-plants-api-openapi.yml
  format: yaml
  label: TwitterAPI.io Plants API
  slug: twitterapi-io-plants-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitterapi-io/openapi/twitterapi-io-plants-api-openapi.yml
- filename: twitterapi-io-twitter-api-openapi.yml
  format: yaml
  label: TwitterAPI.io Twitter API
  slug: twitterapi-io-twitter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twitterapi-io/openapi/twitterapi-io-twitter-api-openapi.yml
auth_types: []
description: Authentication for twitterapi.io requires an API key.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Twitterapi Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: TwitterAPI.io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: TwitterAPI.io
provider_slug: twitterapi-io
scheme_count: 2
schemes:
- evidence: 'Authenticate every twitterapi.io request by sending your API key in the x-api-key header (or as Authorization: Bearer).'
  header: x-api-key
  how_to_obtain: Log in to the TwitterApiIO Dashboard and copy the API key displayed on the dashboard homepage.
  location: header
  name: API Key
  type: apiKey
- evidence: 'If your tool or platform can only send credentials as a Bearer token, you can send the same API key in the `Authorization` header instead:'
  header: Authorization
  how_to_obtain: Log in to the TwitterApiIO Dashboard and copy the API key displayed on the dashboard homepage.
  location: header
  name: Bearer Token
  type: http-bearer
slug: twitterapi-io-authentication
source_filename: twitterapi-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.twitterapi.io/authentication.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.twitterapi.io/authentication.md\nsources:\n- https://docs.twitterapi.io/authentication.md\n- https://docs.twitterapi.io/quickstart.md\ndescription: Authentication for twitterapi.io requires an API key.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Authenticate every twitterapi.io request by sending your API key in the x-api-key header (or as Authorization: Bearer).'\n  location: header\n  header: x-api-key\n  how_to_obtain: Log in to the TwitterApiIO Dashboard and copy the API key displayed on the dashboard homepage.\n- type: http-bearer\n  name: Bearer Token\n  evidence: 'If your tool or platform can only send credentials as a Bearer token, you can send the same API key in the `Authorization` header\n    instead:'\n  location: header\n  header: Authorization\n  how_to_obtain: Log in to the TwitterApiIO Dashboard and copy the API key displayed on the dashboard\
  \ homepage.\nnote: Both schemes use the same API key; if both headers are present, `x-api-key` is used.\ndocs: https://docs.twitterapi.io/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/twitterapi-io/authentication/twitterapi-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- X-API
- Data-Provider
- REST
- Third-Party
---
