---
anonymous_access: false
api_key_in: []
api_specs:
- filename: frely-cloud-openapi-generated.yml
  format: yaml
  label: Frely API
  slug: frely-cloud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/frely-cloud/openapi/_ae-authored/frely-cloud-openapi-generated.yml
auth_types: []
description: Frely authenticates API requests using an API key sent as a bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Frely Authentication
name_suffix: Authentication
oauth_flows: []
overview: Frely declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Frely
provider_slug: frely-cloud
scheme_count: 1
schemes:
- evidence: 'Send your API key as a bearer token: Authorization: Bearer <your key>.'
  header: Authorization
  how_to_obtain: Open the API key page in your console and create one.
  location: header
  name: Bearer
  type: http-bearer
slug: frely-cloud-authentication
source_filename: frely-cloud-authentication.yml
source_heading: Authentication Profile
source_url: https://frely.cloud/docs/faq/using-models.md
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://frely.cloud/docs/faq/using-models.md\nsources:\n- https://frely.cloud/docs/faq/using-models.md\n- https://frely.cloud/docs/\ndescription: Frely authenticates API requests using an API key sent as a bearer token.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send your API key as a bearer token: Authorization: Bearer <your key>.'\n  location: header\n  header: Authorization\n  how_to_obtain: Open the API key page in your console and create one.\nnote: No OAuth2, apiKey, http-basic, or other authentication schemes are documented on the provided pages.\ndocs: https://frely.cloud/docs/faq/using-models.md\n"
source_yaml_url: https://artifacts.apis.io/frely-cloud/authentication/frely-cloud-authentication.yml
summary_line: 1 scheme
tags:
- AI Integration
- Computer access
---
