---
anonymous_access: false
api_key_in: []
api_specs:
- filename: edge-network-assist-api-openapi.yml
  format: yaml
  label: Edge Network Assist API
  slug: edge-network-assist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-assist-api-openapi.yml
- filename: edge-network-cdn-api-openapi.yml
  format: yaml
  label: Edge Network CDN API
  slug: edge-network-cdn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-cdn-api-openapi.yml
- filename: edge-network-compute-api-openapi.yml
  format: yaml
  label: Edge Network Compute API
  slug: edge-network-compute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-compute-api-openapi.yml
- filename: edge-network-deploy-api-openapi.yml
  format: yaml
  label: Edge Network Deploy API
  slug: edge-network-deploy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-deploy-api-openapi.yml
- filename: edge-network-discovery-api-openapi.yml
  format: yaml
  label: Edge Network Discovery API
  slug: edge-network-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-discovery-api-openapi.yml
- filename: edge-network-dns-api-openapi.yml
  format: yaml
  label: Edge Network DNS API
  slug: edge-network-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-dns-api-openapi.yml
- filename: edge-network-projects-api-openapi.yml
  format: yaml
  label: Edge Network Projects API
  slug: edge-network-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-projects-api-openapi.yml
- filename: edge-network-shield-api-openapi.yml
  format: yaml
  label: Edge Network Shield API
  slug: edge-network-shield-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-shield-api-openapi.yml
- filename: edge-network-signup-api-openapi.yml
  format: yaml
  label: Edge Network Signup API
  slug: edge-network-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-signup-api-openapi.yml
- filename: edge-network-storage-api-openapi.yml
  format: yaml
  label: Edge Network Storage API
  slug: edge-network-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/edge-network/openapi/edge-network-storage-api-openapi.yml
auth_types: []
description: Edge Network authentication methods
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Edge Network Authentication
name_suffix: Authentication
oauth_flows: []
overview: Edge Network declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Edge Network
provider_slug: edge-network
scheme_count: 2
schemes:
- evidence: 'Pass the agent access code as a Bearer token:'
  header: Authorization
  how_to_obtain: Create an Agent Access Code in the Account → Agent Access section; the generated code (format ea_live_{random_64_hex}) is shown once and must be stored securely.
  location: header
  name: Agent Access Code
  type: http-bearer
- evidence: Every request to the REST API is authenticated with an API key passed as a Bearer token.
  header: Authorization
  how_to_obtain: Create an API key in the Account → API Keys section; the key (prefix ek_live_) is shown only once and can have optional expiry.
  location: header
  name: API Key
  type: http-bearer
slug: edge-network-authentication
source_filename: edge-network-authentication.yml
source_heading: Authentication Profile
source_url: https://edge.network/docs/agent/access-codes
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://edge.network/docs/agent/access-codes\nsources:\n- https://edge.network/docs/agent/access-codes\n- https://edge.network/docs/account/two-factor-authentication.md\n- https://edge.network/docs/api/authentication.md\n- https://edge.network/docs/cli/authentication.md\ndescription: Edge Network authentication methods\nschemes:\n- type: http-bearer\n  name: Agent Access Code\n  evidence: 'Pass the agent access code as a Bearer token:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an Agent Access Code in the Account → Agent Access section; the generated code (format ea_live_{random_64_hex}) is shown\n    once and must be stored securely.\n- type: http-bearer\n  name: API Key\n  evidence: Every request to the REST API is authenticated with an API key passed as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key\
  \ in the Account → API Keys section; the key (prefix ek_live_) is shown only once and can have optional expiry.\nnote: No OAuth2, apiKey, http-basic, jwt, hmac, mtls, or other schemes are documented on the provided pages.\ndocs: https://edge.network/docs/agent/access-codes\n"
source_yaml_url: https://artifacts.apis.io/edge-network/authentication/edge-network-authentication.yml
summary_line: 2 schemes
tags:
- Cloud
- CDN
- Compute
- Storage
- DNS
- Security
- Artificial Intelligence
---
