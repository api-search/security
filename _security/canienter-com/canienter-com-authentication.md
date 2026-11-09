---
anonymous_access: true
api_key_in: []
auth_types: []
description: Authentication for CanIEnter API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Canienter Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: canienter-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: canienter-com
provider_slug: canienter-com
scheme_count: 2
schemes:
- authorize_url: https://api.canienter.com/oauth/authorize
  evidence: Bearer token (this page)
  flows:
  - client_credentials
  header: Authorization
  how_to_obtain: Register anonymously via POST https://api.canienter.com/oauth/register to receive client_id and client_secret, then exchange them at the token endpoint using client_credentials grant.
  location: header
  name: Bearer token
  scopes:
  - visa:check
  token_url: https://api.canienter.com/oauth/token
  type: http-bearer
- evidence: Anonymous free | none
  how_to_obtain: No credentials required; simply call the free endpoint.
  name: Anonymous free tier
  type: none
slug: canienter-com-authentication
source_filename: canienter-com-authentication.yml
source_heading: Authentication Profile
source_url: https://api.canienter.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.canienter.com/.well-known/oauth-authorization-server\nsources:\n- https://api.canienter.com/.well-known/oauth-authorization-server\n- https://api.canienter.com/auth.md\ndescription: Authentication for CanIEnter API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Bearer token (this page)\n  location: header\n  header: Authorization\n  flows:\n  - client_credentials\n  token_url: https://api.canienter.com/oauth/token\n  authorize_url: https://api.canienter.com/oauth/authorize\n  scopes:\n  - visa:check\n  how_to_obtain: Register anonymously via POST https://api.canienter.com/oauth/register to receive client_id and client_secret, then exchange\n    them at the token endpoint using client_credentials grant.\n- type: none\n  name: Anonymous free tier\n  evidence: Anonymous free | none\n  how_to_obtain: No credentials required; simply call the free endpoint.\n\
  docs: https://api.canienter.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/canienter-com/authentication/canienter-com-authentication.yml
summary_line: 2 schemes
tags:
- Visa checks
- Entry requirements
- Travel
- Data Service
- Immigration
---
