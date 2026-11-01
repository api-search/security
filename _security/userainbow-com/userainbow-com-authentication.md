---
anonymous_access: false
api_key_in: []
api_specs:
- filename: userainbow-com-agency-api-openapi.yml
  format: yaml
  label: Rainbow Agency API
  slug: userainbow-com-agency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userainbow-com/openapi/userainbow-com-agency-api-openapi.yml
- filename: userainbow-com-appetite-api-openapi.yml
  format: yaml
  label: Rainbow Appetite API
  slug: userainbow-com-appetite-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userainbow-com/openapi/userainbow-com-appetite-api-openapi.yml
- filename: userainbow-com-indication-api-openapi.yml
  format: yaml
  label: Rainbow Indication API
  slug: userainbow-com-indication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/userainbow-com/openapi/userainbow-com-indication-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Userainbow Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rainbow declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Rainbow
provider_slug: userainbow-com
scheme_count: 1
schemes:
- evidence: Every request to the API must be accompanied by an API key for validation. This API key can be retrieved from your contact at Rainbow (please message <support@rainbow.com> if you can’t find your contact). It should be attached to the headers in the `Authorization` field in this format `bearer {API Key}`.
  header: Authorization
  how_to_obtain: Contact your Rainbow liaison or email support@rainbow.com to receive the API key.
  location: header
  name: API Key
  type: apiKey
slug: userainbow-com-authentication
source_filename: userainbow-com-authentication.yml
source_heading: Authentication Profile
source_url: https://apidocs.userainbow.com/docs/authentication
source_yaml: "generated: '2026-10-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://apidocs.userainbow.com/docs/authentication\nsources:\n- https://apidocs.userainbow.com/docs/authentication\n- https://apidocs.userainbow.com/docs/quick-start\ndescription: Authentication\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Every request to the API must be accompanied by an API key for validation. This API key can be retrieved from your contact at Rainbow\n    (please message <support@rainbow.com> if you can’t find your contact). It should be attached to the headers in the `Authorization` field in\n    this format `bearer {API Key}`.\n  location: header\n  header: Authorization\n  how_to_obtain: Contact your Rainbow liaison or email support@rainbow.com to receive the API key.\nnote: No OAuth2, http-bearer, or other authentication schemes are documented.\ndocs: https://apidocs.userainbow.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/userainbow-com/authentication/userainbow-com-authentication.yml
summary_line: 1 scheme
tags:
- Insurance
- Restaurants
- Commercial Real Estate
- Beauty & Wellness
- Agents
- MGA
---
