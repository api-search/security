---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lona-agency-openapi-generated.yml
  format: yaml
  label: LONA API
  slug: lona-agency-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lona-agency/openapi/_ae-authored/lona-agency-openapi-generated.yml
auth_types: []
description: Authentication for LONA API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: LONA Authentication
name_suffix: Authentication
oauth_flows: []
overview: LONA declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LONA
provider_slug: lona-agency
scheme_count: 2
schemes:
- evidence: 'Authorization: Bearer <token> can be used instead of X-API-Key . The X-User-Id header is still required.'
  header: Authorization
  how_to_obtain: Obtained from the registration endpoint (/api/v1/agents/register) which returns a service token.
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'Authorization: Bearer <registration-secret> is also accepted for this registration request.'
  header: Authorization
  how_to_obtain: Generated as a registration secret (at least 32 characters) configured on the gateway (AGENT_REGISTRATION_SECRET).
  location: header
  name: Authorization
  type: http-bearer
slug: lona-agency-authentication
source_filename: lona-agency-authentication.yml
source_heading: Authentication Profile
source_url: https://www.lona.agency/docs/getting-started
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.lona.agency/docs/getting-started\nsources:\n- https://www.lona.agency/docs/getting-started\n- https://www.lona.agency/docs/agents/agent-onboarding\ndescription: Authentication for LONA API\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Authorization: Bearer <token> can be used instead of X-API-Key . The X-User-Id header is still required.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtained from the registration endpoint (/api/v1/agents/register) which returns a service token.\n- type: http-bearer\n  name: Authorization\n  evidence: 'Authorization: Bearer <registration-secret> is also accepted for this registration request.'\n  location: header\n  header: Authorization\n  how_to_obtain: Generated as a registration secret (at least 32 characters) configured on the gateway (AGENT_REGISTRATION_SECRET).\nnote: No OAuth2 flows are\
  \ documented. 2 extracted row(s) were dropped because their quote was not on the page.\ndocs: https://www.lona.agency/docs/getting-started\n"
source_yaml_url: https://artifacts.apis.io/lona-agency/authentication/lona-agency-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Trading
- Artificial Intelligence
- Backtesting
- No-Code
---
