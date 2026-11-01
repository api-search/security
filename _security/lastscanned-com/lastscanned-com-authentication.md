---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lastscanned-com-account-api-openapi.yml
  format: yaml
  label: lastscanned Account API
  slug: lastscanned-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastscanned-com/openapi/lastscanned-com-account-api-openapi.yml
- filename: lastscanned-com-carriers-api-openapi.yml
  format: yaml
  label: lastscanned Carriers API
  slug: lastscanned-com-carriers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastscanned-com/openapi/lastscanned-com-carriers-api-openapi.yml
- filename: lastscanned-com-track-api-openapi.yml
  format: yaml
  label: lastscanned Track API
  slug: lastscanned-com-track-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastscanned-com/openapi/lastscanned-com-track-api-openapi.yml
- filename: lastscanned-com-tracking-api-openapi.yml
  format: yaml
  label: lastscanned Tracking API
  slug: lastscanned-com-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastscanned-com/openapi/lastscanned-com-tracking-api-openapi.yml
- filename: lastscanned-com-watches-api-openapi.yml
  format: yaml
  label: lastscanned Watches API
  slug: lastscanned-com-watches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastscanned-com/openapi/lastscanned-com-watches-api-openapi.yml
- filename: lastscanned-com-webhooks-api-openapi.yml
  format: yaml
  label: lastscanned Webhooks API
  slug: lastscanned-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lastscanned-com/openapi/lastscanned-com-webhooks-api-openapi.yml
auth_types: []
description: Authentication for LastScanned API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Lastscanned Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: lastscanned declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: lastscanned
provider_slug: lastscanned-com
scheme_count: 1
schemes:
- evidence: 'Send your key in either header:


    ```http

    Authorization: Bearer lsk_live_…

    ```'
  header: Authorization
  how_to_obtain: Create a key in the dashboard (https://app.lastscanned.com/keys) or with POST /v1/keys.
  location: header
  name: Bearer token
  type: http-bearer
slug: lastscanned-com-authentication
source_filename: lastscanned-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.lastscanned.com/authentication.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.lastscanned.com/authentication.md\nsources:\n- https://docs.lastscanned.com/authentication.md\n- https://docs.lastscanned.com/index.md\ndescription: Authentication for LastScanned API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Send your key in either header:\n\n\n    ```http\n\n    Authorization: Bearer lsk_live_…\n\n    ```'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the dashboard (https://app.lastscanned.com/keys) or with POST /v1/keys.\nnote: No OAuth2 flows, JWT, HMAC, MTLS, or other authentication schemes are documented. 1 extracted row(s) were dropped because their quote was\n  not on the page.\ndocs: https://docs.lastscanned.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/lastscanned-com/authentication/lastscanned-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Tracking
- Logistics
- API
- MCP
---
