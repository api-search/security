---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tandem-cc-com-admin-api-openapi.yml
  format: yaml
  label: Tandem Admin API
  slug: tandem-cc-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-admin-api-openapi.yml
- filename: tandem-cc-com-attachments-api-openapi.yml
  format: yaml
  label: Tandem Attachments API
  slug: tandem-cc-com-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-attachments-api-openapi.yml
- filename: tandem-cc-com-conventions-api-openapi.yml
  format: yaml
  label: Tandem Conventions API
  slug: tandem-cc-com-conventions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-conventions-api-openapi.yml
- filename: tandem-cc-com-drafts-api-openapi.yml
  format: yaml
  label: Tandem Drafts API
  slug: tandem-cc-com-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-drafts-api-openapi.yml
- filename: tandem-cc-com-healthz-api-openapi.yml
  format: yaml
  label: Tandem Healthz API
  slug: tandem-cc-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-healthz-api-openapi.yml
- filename: tandem-cc-com-inbound-api-openapi.yml
  format: yaml
  label: Tandem Inbound API
  slug: tandem-cc-com-inbound-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-inbound-api-openapi.yml
- filename: tandem-cc-com-messages-api-openapi.yml
  format: yaml
  label: Tandem Messages API
  slug: tandem-cc-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-messages-api-openapi.yml
- filename: tandem-cc-com-oauth-api-openapi.yml
  format: yaml
  label: Tandem OAuth API
  slug: tandem-cc-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-oauth-api-openapi.yml
- filename: tandem-cc-com-ops-api-openapi.yml
  format: yaml
  label: Tandem Ops API
  slug: tandem-cc-com-ops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-ops-api-openapi.yml
- filename: tandem-cc-com-passkeys-api-openapi.yml
  format: yaml
  label: Tandem Passkeys API
  slug: tandem-cc-com-passkeys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-passkeys-api-openapi.yml
- filename: tandem-cc-com-preview-api-openapi.yml
  format: yaml
  label: Tandem Preview API
  slug: tandem-cc-com-preview-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-preview-api-openapi.yml
- filename: tandem-cc-com-public-api-openapi.yml
  format: yaml
  label: Tandem Public API
  slug: tandem-cc-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-public-api-openapi.yml
- filename: tandem-cc-com-threads-api-openapi.yml
  format: yaml
  label: Tandem Threads API
  slug: tandem-cc-com-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tandem-cc-com/openapi/tandem-cc-com-threads-api-openapi.yml
auth_types: []
description: Clients authenticate by sending a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Tandem Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tandem declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Tandem
provider_slug: tandem-cc-com
scheme_count: 1
schemes:
- evidence: Use your access token (signup screen or account page ).
  header: Authorization
  how_to_obtain: Grab your access token shown after signing up or on your account page.
  location: header
  name: Bearer token
  type: http-bearer
slug: tandem-cc-com-authentication
source_filename: tandem-cc-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.tandem-cc.com/connect.html
source_yaml: "generated: '2026-11-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.tandem-cc.com/connect.html\nsources:\n- https://www.tandem-cc.com/connect.html\ndescription: Clients authenticate by sending a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Use your access token (signup screen or account page ).\n  location: header\n  header: Authorization\n  how_to_obtain: Grab your access token shown after signing up or on your account page.\nnote: OAuth flows are not described on the page; only the Bearer token method is documented.\ndocs: https://www.tandem-cc.com/connect.html\n"
source_yaml_url: https://artifacts.apis.io/tandem-cc-com/authentication/tandem-cc-com-authentication.yml
summary_line: 1 scheme
tags:
- Communication
- Collaboration
- MCP
---
