---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dynamoi-com-data-api-openapi.yml
  format: yaml
  label: Dynamoi Data API
  slug: dynamoi-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamoi-com/openapi/dynamoi-com-data-api-openapi.yml
auth_types: []
description: Authentication schemes published for Dynamoi
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dynamoi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dynamoi declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Dynamoi
provider_slug: dynamoi-com
scheme_count: 2
schemes:
- authorize_url: https://dynamoi.com/oauth/better-auth/device
  evidence: Dynamoi uses Better Auth OAuth 2.1 for MCP user authorization. The canonical issuer is `https://dynamoi.com/api/auth`, PKCE with `S256` is required, and access tokens are 10-minute JWTs bound to the `https://dynamoi.com/mcp` or `https://dynamoi.com/mcp/directory` resource.
  flows:
  - client_credentials
  - authorization_code
  - device_authorization
  how_to_obtain: Dynamic client registration at https://dynamoi.com/api/auth/oauth2/register for public PKCE clients; device code flow via https://dynamoi.com/api/auth/device/code and user approval at https://dynamoi.com/oauth/better-auth/device.
  name: Dynamoi MCP OAuth
  scopes:
  - dynamoi:read
  - dynamoi:billing.read
  - dynamoi:campaign.write
  - dynamoi:platform.read
  - dynamoi:platform.write
  - dynamoi:distribution.read
  - dynamoi:distribution.apply
  - dynamoi:smart_links.write
  - dynamoi:campaign.launch
  - dynamoi:mcp.full
  type: oauth2
- evidence: 'A monthly subscriber creates a `dmd_` API key in the Dynamoi dashboard and retrieves a dataset family with:

    ```http

    GET https://dynamoi.com/api/data/v1/publications/{publicationId}?format=jsonl

    Authorization: Bearer dmd_<api-key>

    ```'
  header: Authorization
  how_to_obtain: Create a monthly subscription in the Dynamoi dashboard (https://dynamoi.com/dashboard/user/data-api) which generates a `dmd_` API key.
  location: header
  name: Monthly API Key
  type: http-bearer
slug: dynamoi-com-authentication
source_filename: dynamoi-com-authentication.yml
source_heading: Authentication Profile
source_url: https://dynamoi.com/auth.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dynamoi.com/auth.md\nsources:\n- https://dynamoi.com/auth.md\n- https://dynamoi.com/docs/getting-started.md\n- https://dynamoi.com/docs/getting-started/what-is-dynamoi.md\n- https://dynamoi.com/docs/getting-started/onboarding-guide.md\ndescription: Authentication schemes published for Dynamoi\nschemes:\n- type: oauth2\n  name: Dynamoi MCP OAuth\n  evidence: Dynamoi uses Better Auth OAuth 2.1 for MCP user authorization. The canonical issuer is `https://dynamoi.com/api/auth`, PKCE with `S256`\n    is required, and access tokens are 10-minute JWTs bound to the `https://dynamoi.com/mcp` or `https://dynamoi.com/mcp/directory` resource.\n  flows:\n  - client_credentials\n  - authorization_code\n  - device_authorization\n  authorize_url: https://dynamoi.com/oauth/better-auth/device\n  scopes:\n  - dynamoi:read\n  - dynamoi:billing.read\n  - dynamoi:campaign.write\n  - dynamoi:platform.read\n\
  \  - dynamoi:platform.write\n  - dynamoi:distribution.read\n  - dynamoi:distribution.apply\n  - dynamoi:smart_links.write\n  - dynamoi:campaign.launch\n  - dynamoi:mcp.full\n  how_to_obtain: Dynamic client registration at https://dynamoi.com/api/auth/oauth2/register for public PKCE clients; device code flow via https://dynamoi.com/api/auth/device/code\n    and user approval at https://dynamoi.com/oauth/better-auth/device.\n- type: http-bearer\n  name: Monthly API Key\n  evidence: 'A monthly subscriber creates a `dmd_` API key in the Dynamoi dashboard and retrieves a dataset family with:\n\n    ```http\n\n    GET https://dynamoi.com/api/data/v1/publications/{publicationId}?format=jsonl\n\n    Authorization: Bearer dmd_<api-key>\n\n    ```'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a monthly subscription in the Dynamoi dashboard (https://dynamoi.com/dashboard/user/data-api) which generates a `dmd_`\n    API key.\ndocs: https://dynamoi.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/dynamoi-com/authentication/dynamoi-com-authentication.yml
summary_line: 2 schemes
tags:
- Music Promotion
- Spotify
- YouTube
- Distribution
- Analytics
- Independent Artists
- Labels
---
