---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kunkafa-com-account-links-api-openapi.yml
  format: yaml
  label: Kunkafa Account Links API
  slug: kunkafa-com-account-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-account-links-api-openapi.yml
- filename: kunkafa-com-articles-json-api-openapi.yml
  format: yaml
  label: Kunkafa Articles.json API
  slug: kunkafa-com-articles-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-articles-json-api-openapi.yml
- filename: kunkafa-com-authenticated-integrations-api-openapi.yml
  format: yaml
  label: Kunkafa Authenticated integrations API
  slug: kunkafa-com-authenticated-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-authenticated-integrations-api-openapi.yml
- filename: kunkafa-com-glossary-api-openapi.yml
  format: yaml
  label: Kunkafa Glossary API
  slug: kunkafa-com-glossary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-glossary-api-openapi.yml
- filename: kunkafa-com-markets-json-api-openapi.yml
  format: yaml
  label: Kunkafa Markets.json API
  slug: kunkafa-com-markets-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-markets-json-api-openapi.yml
- filename: kunkafa-com-plans-api-openapi.yml
  format: yaml
  label: Kunkafa Plans API
  slug: kunkafa-com-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-plans-api-openapi.yml
- filename: kunkafa-com-plans-json-api-openapi.yml
  format: yaml
  label: Kunkafa Plans.json API
  slug: kunkafa-com-plans-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-plans-json-api-openapi.yml
- filename: kunkafa-com-reports-api-openapi.yml
  format: yaml
  label: Kunkafa Reports API
  slug: kunkafa-com-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-reports-api-openapi.yml
- filename: kunkafa-com-sitemap-markets-xml-api-openapi.yml
  format: yaml
  label: Kunkafa Sitemap Markets.xml API
  slug: kunkafa-com-sitemap-markets-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-sitemap-markets-xml-api-openapi.yml
- filename: kunkafa-com-stats-json-api-openapi.yml
  format: yaml
  label: Kunkafa Stats.json API
  slug: kunkafa-com-stats-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-stats-json-api-openapi.yml
- filename: kunkafa-com-well-known-api-openapi.yml
  format: yaml
  label: Kunkafa .well Known API
  slug: kunkafa-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-well-known-api-openapi.yml
- filename: kunkafa-com-widgets-api-openapi.yml
  format: yaml
  label: Kunkafa Widgets API
  slug: kunkafa-com-widgets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kunkafa-com/openapi/kunkafa-com-widgets-api-openapi.yml
auth_types: []
description: Authentication methods for Kunkafa API and MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Kunkafa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kunkafa declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Kunkafa
provider_slug: kunkafa-com
scheme_count: 2
schemes:
- evidence: 'Send it in the Authorization: Bearer header.'
  header: Authorization
  how_to_obtain: Create API token in Account → API & MCP connections, give it a name, select permissions, token is shown once and expires after 90 days.
  location: header
  name: Bearer token
  type: http-bearer
- authorize_url: https://kunkafa.com/oauth
  evidence: Use authorization code flow with PKCE and resource https://kunkafa.com/mcp.
  flows:
  - authorization_code
  how_to_obtain: Use authorization code flow with PKCE and resource https://kunkafa.com/mcp; discovery starts at https://kunkafa.com/.well-known/oauth-protected-resource/mcp.
  name: OAuth2 Authorization Code with PKCE
  scopes:
  - markets:read
  - outlooks:read
  - performance:read
  - results:read
  - usage:read
  - following:write
  type: oauth2
slug: kunkafa-com-authentication
source_filename: kunkafa-com-authentication.yml
source_heading: Authentication Profile
source_url: https://kunkafa.com/developers/setup
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kunkafa.com/developers/setup\nsources:\n- https://kunkafa.com/developers/setup\n- https://kunkafa.com/ar/developers/setup\ndescription: Authentication methods for Kunkafa API and MCP\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Send it in the Authorization: Bearer header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create API token in Account → API & MCP connections, give it a name, select permissions, token is shown once and expires after\n    90 days.\n- type: oauth2\n  name: OAuth2 Authorization Code with PKCE\n  evidence: Use authorization code flow with PKCE and resource https://kunkafa.com/mcp.\n  flows:\n  - authorization_code\n  authorize_url: https://kunkafa.com/oauth\n  scopes:\n  - markets:read\n  - outlooks:read\n  - performance:read\n  - results:read\n  - usage:read\n  - following:write\n  how_to_obtain: Use authorization\
  \ code flow with PKCE and resource https://kunkafa.com/mcp; discovery starts at https://kunkafa.com/.well-known/oauth-protected-resource/mcp.\ndocs: https://kunkafa.com/developers/setup\n"
source_yaml_url: https://artifacts.apis.io/kunkafa-com/authentication/kunkafa-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Finance
- Market Forecasts
- Cryptocurrency
- Predictive Analytics
- Company
---
