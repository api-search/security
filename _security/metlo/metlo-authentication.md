---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes supported by Metlo as defined in its configuration documentation.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Metlo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metlo declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Metlo
provider_slug: metlo
scheme_count: 4
schemes:
- evidence: Basic Auth
  name: basic
  type: http-basic
- evidence: Header
  header: X-API-KEY
  location: header
  name: header
  type: apiKey
- evidence: JWT
  header: Authorization
  location: header
  name: jwt
  type: jwt
- evidence: Session Cookie
  header: _session_key
  location: cookie
  name: session_cookie
  type: other
slug: metlo-authentication
source_filename: metlo-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.metlo.com/inventory/configuration.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.metlo.com/inventory/configuration.md\nsources:\n- https://docs.metlo.com/inventory/configuration.md\n- https://docs.metlo.com/testing/auth-tests/testing-config.md\n- https://docs.metlo.com/testing/auth-tests/generating-auth-tests.md\n- https://docs.metlo.com/intro/getting-started.md\ndescription: Authentication schemes supported by Metlo as defined in its configuration documentation.\nschemes:\n- type: http-basic\n  name: basic\n  evidence: Basic Auth\n- type: apiKey\n  name: header\n  evidence: Header\n  location: header\n  header: X-API-KEY\n- type: jwt\n  name: jwt\n  evidence: JWT\n  location: header\n  header: Authorization\n- type: other\n  name: session_cookie\n  evidence: Session Cookie\n  location: cookie\n  header: _session_key\nnote: OAuth flows, token URLs, and scopes are not documented for Metlo; therefore they are omitted.\ndocs: https://docs.metlo.com/inventory/configuration.md\n"
source_yaml_url: https://artifacts.apis.io/metlo/authentication/metlo-authentication.yml
summary_line: 4 schemes
tags:
- API Security
- Cloud-Native
- Real-Time Monitoring
- OpenAPI
- CI/CD Integration
---
