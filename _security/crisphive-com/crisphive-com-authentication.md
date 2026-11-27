---
anonymous_access: false
api_key_in: []
api_specs:
- filename: crisphive-com-openapi-generated.yml
  format: yaml
  label: Crisphive API
  slug: crisphive-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crisphive-com/openapi/_ae-authored/crisphive-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Crisphive APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Crisphive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crisphive declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Crisphive
provider_slug: crisphive-com
scheme_count: 2
schemes:
- evidence: Authentication Requests are authenticated with a secret API key sent as a bearer token on every call. The Authorization header Include your API key as a bearer token.
  header: Authorization
  how_to_obtain: Create keys from the dashboard under Settings → Developers; the key value is shown once at creation.
  location: header
  name: API Key
  type: http-bearer
- authorize_url: /oauth/authorize
  evidence: Let your users connect their own Crisphive business to your product — OAuth 2.1 with a consent screen, no API key ever copied.
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Register a client dynamically via POST /oauth/register to receive a client_id (and secret for verified partners). Then follow the authorization code flow.
  name: OAuth 2.1
  scopes:
  - customers_view
  - job_view
  type: oauth2
slug: crisphive-com-authentication
source_filename: crisphive-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.crisphive.com/docs/login-and-api-keys
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.crisphive.com/docs/login-and-api-keys\nsources:\n- https://docs.crisphive.com/docs/login-and-api-keys\n- https://docs.crisphive.com/docs/authentication\n- https://docs.crisphive.com/docs/oauth\n- https://docs.crisphive.com/technical-reference/authentication\ndescription: Authentication methods for Crisphive APIs\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Authentication Requests are authenticated with a secret API key sent as a bearer token on every call. The Authorization header Include\n    your API key as a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys from the dashboard under Settings → Developers; the key value is shown once at creation.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Let your users connect their own Crisphive business to your product — OAuth 2.1 with a consent screen, no API key ever\
  \ copied.\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: /oauth/authorize\n  scopes:\n  - customers_view\n  - job_view\n  how_to_obtain: Register a client dynamically via POST /oauth/register to receive a client_id (and secret for verified partners). Then follow\n    the authorization code flow.\nnote: All URLs are taken directly from the documentation and are relative to the Crisphive API host.\ndocs: https://docs.crisphive.com/docs/login-and-api-keys\n"
source_yaml_url: https://artifacts.apis.io/crisphive-com/authentication/crisphive-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Scheduling
- Field Service Management
- Dispatch
---
