---
anonymous_access: false
api_key_in: []
api_specs:
- filename: flyitalyadsb-live-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Live API
  slug: flyitalyadsb-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-live-api-openapi.yml
- filename: flyitalyadsb-account-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Account API
  slug: flyitalyadsb-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-account-api-openapi.yml
- filename: flyitalyadsb-events-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Events API
  slug: flyitalyadsb-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-events-api-openapi.yml
- filename: flyitalyadsb-flights-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Flights API
  slug: flyitalyadsb-flights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-flights-api-openapi.yml
- filename: flyitalyadsb-history-api-openapi.yml
  format: yaml
  label: FlyItalyADSB History API
  slug: flyitalyadsb-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-history-api-openapi.yml
- filename: flyitalyadsb-keys-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Keys API
  slug: flyitalyadsb-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-keys-api-openapi.yml
- filename: flyitalyadsb-live-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Live API
  slug: flyitalyadsb-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-live-api-openapi.yml
- filename: flyitalyadsb-watch-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Watch API
  slug: flyitalyadsb-watch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-watch-api-openapi.yml
- filename: flyitalyadsb-webhooks-api-openapi.yml
  format: yaml
  label: FlyItalyADSB Webhooks API
  slug: flyitalyadsb-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flyitalyadsb/openapi/flyitalyadsb-webhooks-api-openapi.yml
auth_types: []
description: Authentication methods for FlyItalyADSB API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: FlyItalyADSB Authentication
name_suffix: Authentication
oauth_flows: []
overview: FlyItalyADSB declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: FlyItalyADSB
provider_slug: flyitalyadsb
scheme_count: 3
schemes:
- evidence: 'Send it with every request, in the `X-Api-Key` header:'
  header: X-Api-Key
  how_to_obtain: Use the form on the REST API page or POST to https://api.flyitalyadsb.com/v2/keys as described in the documentation.
  location: header
  name: API key
  type: apiKey
- authorize_url: https://flyitalyadsb.com/authorize
  evidence: 'Assistants with OAuth connectors connect to https://flyitalyadsb.com/mcp with **Connect**: enter your email, then the 6‑digit code you receive, and press **Allow**.'
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Register a client (dynamic registration at https://flyitalyadsb.com/oauth/register) and perform the authorization code flow with PKCE S256.
  location: header
  name: OAuth 2.1
  scopes:
  - mcp
  - offline_access
  type: http-bearer
- evidence: An AI agent that only knows your email can ask for access without a browser redirect, following auth.md.
  header: Authorization
  how_to_obtain: POST to https://flyitalyadsb.com/oauth/agent/identity with the user's email, then follow the verification_uri/user_code ceremony and poll https://flyitalyadsb.com/oauth/token for an access token.
  location: header
  name: Agent registration (auth.md)
  type: other
slug: flyitalyadsb-authentication
source_filename: flyitalyadsb-authentication.yml
source_heading: Authentication Profile
source_url: https://flyitalyadsb.com/data/api/docs/authentication.md
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://flyitalyadsb.com/data/api/docs/authentication.md\nsources:\n- https://flyitalyadsb.com/data/api/docs/authentication.md\n- https://flyitalyadsb.com/data/api/docs/authentication/\n- https://flyitalyadsb.com/auth.md\n- https://flyitalyadsb.com/data/api/docs/quickstart.md\ndescription: Authentication methods for FlyItalyADSB API\nschemes:\n- type: apiKey\n  name: API key\n  evidence: 'Send it with every request, in the `X-Api-Key` header:'\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Use the form on the REST API page or POST to https://api.flyitalyadsb.com/v2/keys as described in the documentation.\n- type: http-bearer\n  name: OAuth 2.1\n  evidence: 'Assistants with OAuth connectors connect to https://flyitalyadsb.com/mcp with **Connect**: enter your email, then the 6‑digit code\n    you receive, and press **Allow**.'\n  location: header\n  header: Authorization\n\
  \  flows:\n  - authorization_code\n  authorize_url: https://flyitalyadsb.com/authorize\n  scopes:\n  - mcp\n  - offline_access\n  how_to_obtain: Register a client (dynamic registration at https://flyitalyadsb.com/oauth/register) and perform the authorization code flow with\n    PKCE S256.\n- type: other\n  name: Agent registration (auth.md)\n  evidence: An AI agent that only knows your email can ask for access without a browser redirect, following auth.md.\n  location: header\n  header: Authorization\n  how_to_obtain: POST to https://flyitalyadsb.com/oauth/agent/identity with the user's email, then follow the verification_uri/user_code ceremony\n    and poll https://flyitalyadsb.com/oauth/token for an access token.\ndocs: https://flyitalyadsb.com/data/api/docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/flyitalyadsb/authentication/flyitalyadsb-authentication.yml
summary_line: 3 schemes
tags:
- ADS-B
- MLAT
- Aviation
- Flight Tracking
- Open Data
---
