---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gluecron-com-openapi-generated.yml
  format: yaml
  label: Merjax API
  slug: gluecron-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gluecron-com/openapi/_ae-authored/gluecron-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Merjax API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Merjax Authentication
name_suffix: Authentication
oauth_flows: []
overview: Merjax declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Merjax
provider_slug: gluecron-com
scheme_count: 1
schemes:
- evidence: Authenticated endpoints require a Bearer token in the Authorization header.
  header: Authorization
  how_to_obtain: Generate a personal access token at /settings/tokens . Tokens start with glc_ and are shown only once.
  location: header
  name: Personal Access Token
  type: http-bearer
slug: gluecron-com-authentication
source_filename: gluecron-com-authentication.yml
source_heading: Authentication Profile
source_url: https://gluecron.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gluecron.com/.well-known/oauth-authorization-server\nsources:\n- https://gluecron.com/.well-known/oauth-authorization-server\n- https://gluecron.com/.well-known/oauth-protected-resource\n- https://gluecron.com/docs/api\n- https://gluecron.com/docs/getting-started\ndescription: Authentication methods for Merjax API\nschemes:\n- type: http-bearer\n  name: Personal Access Token\n  evidence: Authenticated endpoints require a Bearer token in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a personal access token at /settings/tokens . Tokens start with glc_ and are shown only once.\ndocs: https://gluecron.com/.well-known/oauth-authorization-server\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/gluecron-com/authentication/gluecron-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Version Control
- DevOps
- Platform
- Open Source
---
