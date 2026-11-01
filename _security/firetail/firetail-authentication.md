---
anonymous_access: false
api_key_in: []
api_specs:
- filename: firetail-openapi-generated.yml
  format: yaml
  label: FireTail API
  slug: firetail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firetail/openapi/_ae-authored/firetail-openapi-generated.yml
auth_types: []
description: Authentication schemes published on the FireTail API documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Firetail Authentication
name_suffix: Authentication
oauth_flows: []
overview: FireTail declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FireTail
provider_slug: firetail
scheme_count: 1
schemes:
- evidence: The FireTail API uses JWT tokens obtained through OAuth 2.0 client credentials flow.
  how_to_obtain: Client credentials can be managed through your FireTail organization settings and are sent in the token request body as form‑encoded parameters (grant_type, client_id, client_secret).
  name: OAuth 2.0 client credentials
  token_url: https://api.saas.eu-west-1.prod.firetail.app/oauth/token
  type: oauth2
slug: firetail-authentication
source_filename: firetail-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.firetail.ai/api/authentication
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.firetail.ai/api/authentication\nsources:\n- https://docs.firetail.ai/api/authentication\n- https://docs.firetail.ai/docs/organizations/reset-multifactor-authentication\n- https://docs.firetail.ai/docs/findings/ai-workforce-credential-leakage\n- https://docs.firetail.ai/docs/findings/ai-glitch\ndescription: Authentication schemes published on the FireTail API documentation.\nschemes:\n- type: oauth2\n  name: OAuth 2.0 client credentials\n  evidence: The FireTail API uses JWT tokens obtained through OAuth 2.0 client credentials flow.\n  token_url: https://api.saas.eu-west-1.prod.firetail.app/oauth/token\n  how_to_obtain: Client credentials can be managed through your FireTail organization settings and are sent in the token request body as form‑encoded\n    parameters (grant_type, client_id, client_secret).\ndocs: https://docs.firetail.ai/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/firetail/authentication/firetail-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Security
- Governance
- Platform
- Cloud
---
