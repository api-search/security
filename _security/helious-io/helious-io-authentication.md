---
anonymous_access: false
api_key_in: []
api_specs:
- filename: helious-io-agent-sign-in-and-a2a-api-openapi.yml
  format: yaml
  label: Helious Agent sign-in and A2A API
  slug: helious-io-agent-sign-in-and-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-agent-sign-in-and-a2a-api-openapi.yml
- filename: helious-io-ask-helious-api-openapi.yml
  format: yaml
  label: Helious Ask Helious API
  slug: helious-io-ask-helious-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-ask-helious-api-openapi.yml
- filename: helious-io-boards-api-openapi.yml
  format: yaml
  label: Helious Boards API
  slug: helious-io-boards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-boards-api-openapi.yml
- filename: helious-io-economic-data-api-openapi.yml
  format: yaml
  label: Helious Economic data API
  slug: helious-io-economic-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-economic-data-api-openapi.yml
- filename: helious-io-news-and-feed-api-openapi.yml
  format: yaml
  label: Helious News and feed API
  slug: helious-io-news-and-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-news-and-feed-api-openapi.yml
- filename: helious-io-rates-and-curve-api-openapi.yml
  format: yaml
  label: Helious Rates and curve API
  slug: helious-io-rates-and-curve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-rates-and-curve-api-openapi.yml
- filename: helious-io-reference-api-openapi.yml
  format: yaml
  label: Helious Reference API
  slug: helious-io-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-reference-api-openapi.yml
- filename: helious-io-series-api-openapi.yml
  format: yaml
  label: Helious Series API
  slug: helious-io-series-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-series-api-openapi.yml
- filename: helious-io-the-fed-api-openapi.yml
  format: yaml
  label: Helious The Fed API
  slug: helious-io-the-fed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-the-fed-api-openapi.yml
- filename: helious-io-the-squawk-api-openapi.yml
  format: yaml
  label: Helious The squawk API
  slug: helious-io-the-squawk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-the-squawk-api-openapi.yml
- filename: helious-io-treasury-auctions-api-openapi.yml
  format: yaml
  label: Helious Treasury auctions API
  slug: helious-io-treasury-auctions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-treasury-auctions-api-openapi.yml
- filename: helious-io-your-key-api-openapi.yml
  format: yaml
  label: Helious Your key API
  slug: helious-io-your-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/helious-io/openapi/helious-io-your-key-api-openapi.yml
auth_types: []
description: Authentication methods for Helious as documented
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Helious Authentication
name_suffix: Authentication
oauth_flows: []
overview: Helious declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Helious
provider_slug: helious-io
scheme_count: 3
schemes:
- evidence: Send no credential. 1 day of history, news one hour behind, no market prices, 30 requests a minute shared per network address.
  how_to_obtain: No credential required; endpoints return data anonymously.
  name: anonymous
  type: other
- authorize_url: https://helious.io/oauth/authorize
  evidence: Authorization code with PKCE S256 and dynamic client registration.
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: POST https://api.helious.io/oauth/register to obtain client_id, then send user to consent screen, exchange code at token endpoint.
  location: header
  name: oauth
  scopes:
  - market:read
  - account:read
  - openid
  - offline_access
  type: oauth2
- evidence: A long-lived key the person creates on their account page and gives to the agent.
  header: Authorization
  how_to_obtain: Person creates a key via POST https://api.helious.io/api/me/api-keys using their signed‑in session.
  location: header
  name: api_key
  type: http-bearer
slug: helious-io-authentication
source_filename: helious-io-authentication.yml
source_heading: Authentication Profile
source_url: https://helious.io/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://helious.io/.well-known/oauth-authorization-server\nsources:\n- https://helious.io/.well-known/oauth-authorization-server\n- https://helious.io/auth.md\n- https://helious.io/ai/\n- https://api.helious.io/v1/context\ndescription: Authentication methods for Helious as documented\nschemes:\n- type: other\n  name: anonymous\n  evidence: Send no credential. 1 day of history, news one hour behind, no market prices, 30 requests a minute shared per network address.\n  how_to_obtain: No credential required; endpoints return data anonymously.\n- type: oauth2\n  name: oauth\n  evidence: Authorization code with PKCE S256 and dynamic client registration.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://helious.io/oauth/authorize\n  scopes:\n  - market:read\n  - account:read\n  - openid\n  - offline_access\n  how_to_obtain: POST https://api.helious.io/oauth/register\
  \ to obtain client_id, then send user to consent screen, exchange code at token endpoint.\n- type: http-bearer\n  name: api_key\n  evidence: A long-lived key the person creates on their account page and gives to the agent.\n  location: header\n  header: Authorization\n  how_to_obtain: Person creates a key via POST https://api.helious.io/api/me/api-keys using their signed‑in session.\ndocs: https://helious.io/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/helious-io/authentication/helious-io-authentication.yml
summary_line: 3 schemes
tags:
- Finance
- Market Data
- News
- Economic Calendar
- Treasury
---
