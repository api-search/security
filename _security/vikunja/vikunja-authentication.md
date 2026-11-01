---
anonymous_access: false
api_key_in: []
api_specs:
- filename: vikunja-openapi-generated.yml
  format: yaml
  label: Vikunja API
  slug: vikunja-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vikunja/openapi/_ae-authored/vikunja-openapi-generated.yml
auth_types: []
description: Authentication methods published on Vikunja documentation pages.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Vikunja Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vikunja declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Vikunja
provider_slug: vikunja
scheme_count: 1
schemes:
- authorize_url: /oauth/authorize
  evidence: Vikunja can act as an OAuth 2.0 Authorization Server, implementing the Authorization Code flow with mandatory PKCE (Proof Key for Code Exchange, S256 only).
  flows:
  - authorization_code
  how_to_obtain: No client registration is required. The client_id can be any string chosen by the integrator; it must be consistent between the authorization and token exchange steps.
  name: Vikunja OAuth2 Authorization Code
  type: oauth2
slug: vikunja-authentication
source_filename: vikunja-authentication.yml
source_heading: Authentication Profile
source_url: https://vikunja.io/docs/ldap/
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://vikunja.io/docs/ldap/\nsources:\n- https://vikunja.io/docs/ldap/\n- https://vikunja.io/docs/oauth-server/\n- https://vikunja.io/docs/fail2ban/\n- https://vikunja.io/docs/metrics-setup/\ndescription: Authentication methods published on Vikunja documentation pages.\nschemes:\n- type: oauth2\n  name: Vikunja OAuth2 Authorization Code\n  evidence: Vikunja can act as an OAuth 2.0 Authorization Server, implementing the Authorization Code flow with mandatory PKCE (Proof Key for\n    Code Exchange, S256 only).\n  flows:\n  - authorization_code\n  authorize_url: /oauth/authorize\n  how_to_obtain: No client registration is required. The client_id can be any string chosen by the integrator; it must be consistent between the\n    authorization and token exchange steps.\ndocs: https://vikunja.io/docs/ldap/\n"
source_yaml_url: https://artifacts.apis.io/vikunja/authentication/vikunja-authentication.yml
summary_line: 1 scheme
tags:
- Company
- OpenSource
- TaskManagement
- SelfHostable
- European
---
