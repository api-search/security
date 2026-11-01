---
anonymous_access: false
api_key_in: []
api_specs:
- filename: feathr-openapi-generated.yml
  format: yaml
  label: Feathr API
  slug: feathr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feathr/openapi/_ae-authored/feathr-openapi-generated.yml
auth_types: []
description: The Feathr API authenticates every request with an opaque API key presented as a bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Feathr Authentication
name_suffix: Authentication
oauth_flows: []
overview: Feathr declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Feathr
provider_slug: feathr
scheme_count: 1
schemes:
- evidence: The Feathr API authenticates every request with an opaque API key presented as a bearer token.
  header: Authorization
  how_to_obtain: API keys are minted from the Feathr app; the key is shown once at creation and cannot be recovered afterward.
  location: header
  name: API key
  type: http-bearer
slug: feathr-authentication
source_filename: feathr-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.feathr.co/authentication/
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.feathr.co/authentication/\nsources:\n- https://docs.feathr.co/authentication/\n- https://docs.feathr.co/getting-started/\ndescription: The Feathr API authenticates every request with an opaque API key presented as a bearer token.\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: The Feathr API authenticates every request with an opaque API key presented as a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: API keys are minted from the Feathr app; the key is shown once at creation and cannot be recovered afterward.\nnote: No OAuth2 or other authentication schemes are documented.\ndocs: https://docs.feathr.co/authentication/\n"
source_yaml_url: https://artifacts.apis.io/feathr/authentication/feathr-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Digital Marketing
- AI
- Nonprofit
- Event Promotion
---
