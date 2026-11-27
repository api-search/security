---
anonymous_access: false
api_key_in: []
api_specs:
- filename: postio-co-uk-address-api-openapi.yml
  format: yaml
  label: Postio Address API
  slug: postio-co-uk-address-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postio-co-uk/openapi/postio-co-uk-address-api-openapi.yml
- filename: postio-co-uk-email-api-openapi.yml
  format: yaml
  label: Postio Email API
  slug: postio-co-uk-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postio-co-uk/openapi/postio-co-uk-email-api-openapi.yml
- filename: postio-co-uk-other-api-openapi.yml
  format: yaml
  label: Postio Other API
  slug: postio-co-uk-other-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postio-co-uk/openapi/postio-co-uk-other-api-openapi.yml
- filename: postio-co-uk-phone-api-openapi.yml
  format: yaml
  label: Postio Phone API
  slug: postio-co-uk-phone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/postio-co-uk/openapi/postio-co-uk-phone-api-openapi.yml
auth_types: []
description: Postio authenticates every request with an API key sent in the x-api-key header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Postio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Postio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Postio
provider_slug: postio-co-uk
scheme_count: 1
schemes:
- evidence: Postio authenticates every request with an API key sent in the x-api-key header.
  header: x-api-key
  how_to_obtain: Copy your key from the dashboard; it looks like pk_ followed by 32 hex characters.
  location: header
  name: API key
  type: apiKey
slug: postio-co-uk-authentication
source_filename: postio-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: https://postio.co.uk/docs/authentication
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://postio.co.uk/docs/authentication\nsources:\n- https://postio.co.uk/docs/authentication\n- https://postio.co.uk/docs\ndescription: Postio authenticates every request with an API key sent in the x-api-key header.\nschemes:\n- type: apiKey\n  name: API key\n  evidence: Postio authenticates every request with an API key sent in the x-api-key header.\n  location: header\n  header: x-api-key\n  how_to_obtain: Copy your key from the dashboard; it looks like pk_ followed by 32 hex characters.\nnote: No OAuth2 or other authentication schemes are documented.\ndocs: https://postio.co.uk/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/postio-co-uk/authentication/postio-co-uk-authentication.yml
summary_line: 1 scheme
tags:
- Company
- United Kingdom
- Address
- Email
- Phone
- Validation
---
