---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openmarkets-openapi-generated.yml
  format: yaml
  label: OpenMarkets Group API
  slug: openmarkets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openmarkets/openapi/_ae-authored/openmarkets-openapi-generated.yml
auth_types: []
description: Openmarkets APIs use OAuth2 client credentials grant. Applications exchange a client ID and secret for a short‑lived bearer token and send it in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Openmarkets Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenMarkets Group declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: OpenMarkets Group
provider_slug: openmarkets
scheme_count: 1
schemes:
- evidence: Every Openmarkets API is protected by OAuth2. Your application exchanges a client ID and secret for a short-lived bearer token, then sends that token on each request.
  flows:
  - client_credentials
  how_to_obtain: Credentials (client_id and client_secret) are issued by Openmarkets during onboarding; contact Openmarkets if you do not have them.
  name: OAuth2 Client Credentials
  scopes:
  - market-data-api
  - news-api
  - oms-api
  - oms-streams-api
  - accounts-submissions
  - accounts-read
  - accounts-manage
  - advice-read
  - back-office-api
  token_url: https://stage-identity.openmarkets.com.au/connect/token
  type: oauth2
slug: openmarkets-authentication
source_filename: openmarkets-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.openmarkets.com.au/authentication
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.openmarkets.com.au/authentication\nsources:\n- https://docs.openmarkets.com.au/authentication\n- https://docs.openmarkets.com.au/quickstart\ndescription: Openmarkets APIs use OAuth2 client credentials grant. Applications exchange a client ID and secret for a short‑lived bearer token\n  and send it in the Authorization header.\nschemes:\n- type: oauth2\n  name: OAuth2 Client Credentials\n  evidence: Every Openmarkets API is protected by OAuth2. Your application exchanges a client ID and secret for a short-lived bearer token, then\n    sends that token on each request.\n  flows:\n  - client_credentials\n  token_url: https://stage-identity.openmarkets.com.au/connect/token\n  scopes:\n  - market-data-api\n  - news-api\n  - oms-api\n  - oms-streams-api\n  - accounts-submissions\n  - accounts-read\n  - accounts-manage\n  - advice-read\n  - back-office-api\n  how_to_obtain:\
  \ Credentials (client_id and client_secret) are issued by Openmarkets during onboarding; contact Openmarkets if you do not have\n    them.\nnote: The token request is authenticated with HTTP Basic authentication where the client_id is the username and the client_secret is the password.\n  The bearer token must be sent in the Authorization header as 'Bearer {access_token}'.\ndocs: https://docs.openmarkets.com.au/authentication\n"
source_yaml_url: https://artifacts.apis.io/openmarkets/authentication/openmarkets-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
