---
anonymous_access: false
api_key_in: []
api_specs:
- filename: capacities-io-blocks-api-openapi.yml
  format: yaml
  label: Capacities Blocks API
  slug: capacities-io-blocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capacities-io/openapi/capacities-io-blocks-api-openapi.yml
- filename: capacities-io-object-api-openapi.yml
  format: yaml
  label: Capacities Object API
  slug: capacities-io-object-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capacities-io/openapi/capacities-io-object-api-openapi.yml
- filename: capacities-io-objects-api-openapi.yml
  format: yaml
  label: Capacities Objects API
  slug: capacities-io-objects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capacities-io/openapi/capacities-io-objects-api-openapi.yml
- filename: capacities-io-space-api-openapi.yml
  format: yaml
  label: Capacities Space API
  slug: capacities-io-space-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/capacities-io/openapi/capacities-io-space-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Capacities Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capacities declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Capacities
provider_slug: capacities-io
scheme_count: 2
schemes:
- evidence: The Capacities API uses Bearer authentication (token-based, OAuth 2.0 RFC 6750).
  header: Authorization
  how_to_obtain: 'Generate a personal token inside the Capacities desktop app: Open Settings → Capacities API → Generate new token.'
  location: header
  name: Personal API token
  type: http-bearer
- authorize_url: https://api.capacities.io/oauth/authorize
  evidence: OAuth 2.0 Use OAuth when you are building an integration, app, or service that other users will connect to their Capacities account.
  flows:
  - authorization_code
  how_to_obtain: Submit integration details via email to receive a client_id; no client secret is issued.
  name: Capacities OAuth
  scopes:
  - api:read
  - api:write
  - offline_access
  type: oauth2
slug: capacities-io-authentication
source_filename: capacities-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.capacities.io/raw/reference/account.md
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.capacities.io/raw/reference/account.md\nsources:\n- https://docs.capacities.io/raw/reference/account.md\n- https://docs.capacities.io/reference/account\n- https://developers.capacities.io/api/overview/authentication\n- https://developers.capacities.io/api/concepts/text-tokens\nschemes:\n- type: http-bearer\n  name: Personal API token\n  evidence: The Capacities API uses Bearer authentication (token-based, OAuth 2.0 RFC 6750).\n  location: header\n  header: Authorization\n  how_to_obtain: 'Generate a personal token inside the Capacities desktop app: Open Settings → Capacities API → Generate new token.'\n- type: oauth2\n  name: Capacities OAuth\n  evidence: OAuth 2.0 Use OAuth when you are building an integration, app, or service that other users will connect to their Capacities account.\n  flows:\n  - authorization_code\n  authorize_url: https://api.capacities.io/oauth/authorize\n\
  \  scopes:\n  - api:read\n  - api:write\n  - offline_access\n  how_to_obtain: Submit integration details via email to receive a client_id; no client secret is issued.\ndocs: https://docs.capacities.io/raw/reference/account.md\n"
source_yaml_url: https://artifacts.apis.io/capacities-io/authentication/capacities-io-authentication.yml
summary_line: 2 schemes
tags:
- Knowledge Management
- Note Taking
- Productivity
- Cross-Platform
- Collaboration
---
