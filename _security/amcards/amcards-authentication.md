---
anonymous_access: false
api_key_in: []
api_specs:
- filename: amcards-openapi-generated.yml
  format: yaml
  label: AMcards API
  slug: amcards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amcards/openapi/_ae-authored/amcards-openapi-generated.yml
auth_types: []
description: Authentication for AMcards API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: AMcards Authentication
name_suffix: Authentication
oauth_flows: []
overview: AMcards declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AMcards
provider_slug: amcards
scheme_count: 2
schemes:
- evidence: You can specify your access token in the Authorization header of your request.
  header: Authorization
  how_to_obtain: Generate an Access Token for your AMcards account via the Connected Applications page.
  location: header
  name: Bearer
  type: http-bearer
- evidence: Your access token that you generated for use with this app. You can also specify your access token in the Authorization header of your request. In that case, do not include it in your POST parameters.
  how_to_obtain: Generate an Access Token for your AMcards account via the Connected Applications page.
  location: body
  name: access_token
  type: apiKey
slug: amcards-authentication
source_filename: amcards-authentication.yml
source_heading: Authentication Profile
source_url: https://amcards.com/docs/2nd-example/
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://amcards.com/docs/2nd-example/\nsources:\n- https://amcards.com/docs/2nd-example/\ndescription: Authentication for AMcards API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: You can specify your access token in the Authorization header of your request.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an Access Token for your AMcards account via the Connected Applications page.\n- type: apiKey\n  name: access_token\n  evidence: Your access token that you generated for use with this app. You can also specify your access token in the Authorization header of\n    your request. In that case, do not include it in your POST parameters.\n  location: body\n  how_to_obtain: Generate an Access Token for your AMcards account via the Connected Applications page.\nnote: No OAuth2 flows are documented on the page.\ndocs: https://amcards.com/docs/2nd-example/\n"
source_yaml_url: https://artifacts.apis.io/amcards/authentication/amcards-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Appreciation-Marketing
- Cards
- Customer Engagement
- Software-as-a-Service
- Marketing
---
