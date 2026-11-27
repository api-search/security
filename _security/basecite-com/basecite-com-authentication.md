---
anonymous_access: false
api_key_in: []
api_specs:
- filename: basecite-com-admin-api-openapi.yml
  format: yaml
  label: BaseCite Admin API
  slug: basecite-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-admin-api-openapi.yml
- filename: basecite-com-ai-api-openapi.yml
  format: yaml
  label: BaseCite AI API
  slug: basecite-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-ai-api-openapi.yml
- filename: basecite-com-oauth-api-openapi.yml
  format: yaml
  label: BaseCite OAuth API
  slug: basecite-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-oauth-api-openapi.yml
- filename: basecite-com-organizations-api-openapi.yml
  format: yaml
  label: BaseCite Organizations API
  slug: basecite-com-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-organizations-api-openapi.yml
- filename: basecite-com-portal-api-openapi.yml
  format: yaml
  label: BaseCite Portal API
  slug: basecite-com-portal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-portal-api-openapi.yml
- filename: basecite-com-sandbox-api-openapi.yml
  format: yaml
  label: BaseCite Sandbox API
  slug: basecite-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-sandbox-api-openapi.yml
auth_types: []
description: BaseCite authentication
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: BaseCite Authentication
name_suffix: Authentication
oauth_flows: []
overview: BaseCite declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: BaseCite
provider_slug: basecite-com
scheme_count: 2
schemes:
- evidence: Send the credential in the documented `x-api-key` header.
  header: x-api-key
  how_to_obtain: Credentials are issued or rotated by BaseCite through the approved administrative or secure secret‑store workflow.
  location: header
  name: Tenant-scoped API key
  type: apiKey
- evidence: OAuth 2.0 client credentials are supported for provisioned tenant clients.
  flows:
  - client_credentials
  how_to_obtain: Discover the authorization server at https://api.basecite.com/.well-known/oauth-authorization-server, then exchange the provisioned client credentials at https://api.basecite.com/oauth/token.
  name: OAuth 2.0 client credentials
  type: oauth2
slug: basecite-com-authentication
source_filename: basecite-com-authentication.yml
source_heading: Authentication Profile
source_url: https://basecite.com/auth.md
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://basecite.com/auth.md\nsources:\n- https://basecite.com/auth.md\ndescription: BaseCite authentication\nschemes:\n- type: apiKey\n  name: Tenant-scoped API key\n  evidence: Send the credential in the documented `x-api-key` header.\n  location: header\n  header: x-api-key\n  how_to_obtain: Credentials are issued or rotated by BaseCite through the approved administrative or secure secret‑store workflow.\n- type: oauth2\n  name: OAuth 2.0 client credentials\n  evidence: OAuth 2.0 client credentials are supported for provisioned tenant clients.\n  flows:\n  - client_credentials\n  how_to_obtain: Discover the authorization server at https://api.basecite.com/.well-known/oauth-authorization-server, then exchange the provisioned\n    client credentials at https://api.basecite.com/oauth/token.\ndocs: https://basecite.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/basecite-com/authentication/basecite-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Evidence
- Platform
- Privacy
---
