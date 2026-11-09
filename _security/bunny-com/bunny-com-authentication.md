---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bunny-com-openapi-generated.yml
  format: yaml
  label: Bunny API
  slug: bunny-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bunny-com/openapi/_ae-authored/bunny-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Bunny API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bunny Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bunny declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bunny
provider_slug: bunny-com
scheme_count: 1
schemes:
- evidence: Generate an OAuth 2.0 access token with the client credentials grant, send it as a Bearer authorization header
  header: Authorization
  how_to_obtain: Create an API client with the required scopes, then POST to the token endpoint with client_id, client_secret and grant_type=client_credentials
  location: header
  name: OAuth 2.0 Bearer
  scopes:
  - standard:read
  - standard:write
  token_url: https://<subdomain>.bunny.com/oauth/token
  type: http-bearer
slug: bunny-com-authentication
source_filename: bunny-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.bunny.com/developer/portal-session-token
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.bunny.com/developer/portal-session-token\nsources:\n- https://docs.bunny.com/developer/portal-session-token\n- https://docs.bunny.com/developer/using-the-graphql-api/authorizing-api-requests\n- https://docs.bunny.com/guide/getting-started/superdesk-sample-saas-co\n- https://docs.bunny.com/guide/tour/product-catalog/product-quick-start\ndescription: Authentication methods for Bunny API\nschemes:\n- type: http-bearer\n  name: OAuth 2.0 Bearer\n  evidence: Generate an OAuth 2.0 access token with the client credentials grant, send it as a Bearer authorization header\n  location: header\n  header: Authorization\n  token_url: https://<subdomain>.bunny.com/oauth/token\n  scopes:\n  - standard:read\n  - standard:write\n  how_to_obtain: Create an API client with the required scopes, then POST to the token endpoint with client_id, client_secret and grant_type=client_credentials\n\
  docs: https://docs.bunny.com/developer/portal-session-token\n"
source_yaml_url: https://artifacts.apis.io/bunny-com/authentication/bunny-com-authentication.yml
summary_line: 1 scheme
tags:
- Billing
- CPQ
- Revenue Recognition
- SaaS Analytics
- Revenue Operations
- Stripe Integration
- AI Agents
---
