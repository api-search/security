---
anonymous_access: false
api_key_in: []
api_specs:
- filename: accoil-accoil-api-api-openapi.yml
  format: yaml
  label: Accoil API
  slug: accoil-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/accoil/openapi/accoil-accoil-api-api-openapi.yml
- filename: accoil-openapi-generated.yml
  format: yaml
  label: Accoil API
  slug: accoil-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/accoil/openapi/_ae-authored/accoil-openapi-generated.yml
auth_types: []
description: Authentication methods for Accoil API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Accoil Authentication
name_suffix: Authentication
oauth_flows: []
overview: Accoil declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Accoil
provider_slug: accoil
scheme_count: 2
schemes:
- evidence: All API requests require authentication via a Bearer token. Provide your API token in the Authorization header of each request.
  header: Authorization
  how_to_obtain: 'You can create and manage your API token by navigating to: Settings > Product Settings > API Token in the Accoil web app.'
  location: header
  name: BearerAuth
  type: http-bearer
- evidence: 'Authorization: Basic YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Find your API key under Account > General in the Accoil dashboard.
  location: header
  name: BasicAuth
  type: http-basic
slug: accoil-authentication
source_filename: accoil-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.accoil.com/docs/accoil-api/workspaces
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.accoil.com/docs/accoil-api/workspaces\nsources:\n- https://developer.accoil.com/docs/accoil-api/workspaces\n- https://developer.accoil.com/docs/quick-start/rest-api\n- https://docs.accoil.com/docs/getting-started\n- https://docs.accoil.com/docs/getting-started/data-sources/sending-data-directly-to-accoil\ndescription: Authentication methods for Accoil API\nschemes:\n- type: http-bearer\n  name: BearerAuth\n  evidence: All API requests require authentication via a Bearer token. Provide your API token in the Authorization header of each request.\n  location: header\n  header: Authorization\n  how_to_obtain: 'You can create and manage your API token by navigating to: Settings > Product Settings > API Token in the Accoil web app.'\n- type: http-basic\n  name: BasicAuth\n  evidence: 'Authorization: Basic YOUR_API_KEY'\n  location: header\n  header: Authorization\n \
  \ how_to_obtain: Find your API key under Account > General in the Accoil dashboard.\nnote: No OAuth2, apiKey, jwt, hmac, mtls, or other authentication schemes are documented on the provided pages.\ndocs: https://developer.accoil.com/docs/accoil-api/workspaces\n"
source_yaml_url: https://artifacts.apis.io/accoil/authentication/accoil-authentication.yml
summary_line: 2 schemes
tags:
- Retention
- Expansion
- Customer Success
- Playbook
- Analytics
---
