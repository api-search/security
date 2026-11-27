---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hepcloud-net-openapi-generated.yml
  format: yaml
  label: HepCloud API
  slug: hepcloud-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hepcloud-net/openapi/_ae-authored/hepcloud-net-openapi-generated.yml
auth_types: []
description: Client authenticates to HepCloud API using a bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: HepCloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: HepCloud declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: HepCloud
provider_slug: hepcloud-net
scheme_count: 1
schemes:
- evidence: 'curl -H "Authorization: Bearer <token>" https://api.hepcloud.net/v1/servers'
  header: Authorization
  how_to_obtain: Created via the HepCloud console under API Tokens → Create token.
  location: header
  name: Bearer token
  type: http-bearer
slug: hepcloud-net-authentication
source_filename: hepcloud-net-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.hepcloud.net/tr/api-tokenlari/
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.hepcloud.net/tr/api-tokenlari/\nsources:\n- https://docs.hepcloud.net/tr/api-tokenlari/\n- https://docs.hepcloud.net/en/api-tokenlari/\ndescription: Client authenticates to HepCloud API using a bearer token.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'curl -H \"Authorization: Bearer <token>\" https://api.hepcloud.net/v1/servers'\n  location: header\n  header: Authorization\n  how_to_obtain: Created via the HepCloud console under API Tokens → Create token.\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the pages.\ndocs: https://docs.hepcloud.net/tr/api-tokenlari/\n"
source_yaml_url: https://artifacts.apis.io/hepcloud-net/authentication/hepcloud-net-authentication.yml
summary_line: 1 scheme
tags:
- Cloud
- Hosting
- PostgreSQL
- Turkish
---
