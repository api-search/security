---
anonymous_access: false
api_key_in: []
api_specs:
- filename: obligationsign-com-openapi-generated.yml
  format: yaml
  label: obligationsign-com API
  slug: obligationsign-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/obligationsign-com/openapi/_ae-authored/obligationsign-com-openapi-generated.yml
auth_types: []
description: ObligationSign uses an API key returned by the auto‑register endpoint as a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Obligationsign Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: obligationsign-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: obligationsign-com
provider_slug: obligationsign-com
scheme_count: 1
schemes:
- evidence: Save your api_key — you'll use it in every subsequent request.
  header: Authorization
  how_to_obtain: POST /auto-register returns an "api_key" field in the JSON response.
  location: header
  name: api_key
  type: http-bearer
slug: obligationsign-com-authentication
source_filename: obligationsign-com-authentication.yml
source_heading: Authentication Profile
source_url: https://obligationsign.com/docs/quickstart/
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://obligationsign.com/docs/quickstart/\nsources:\n- https://obligationsign.com/docs/quickstart/\n- https://www.obligationsign.com/docs/quickstart/\ndescription: ObligationSign uses an API key returned by the auto‑register endpoint as a Bearer token.\nschemes:\n- type: http-bearer\n  name: api_key\n  evidence: Save your api_key — you'll use it in every subsequent request.\n  location: header\n  header: Authorization\n  how_to_obtain: POST /auto-register returns an \"api_key\" field in the JSON response.\nnote: No other authentication mechanisms (apiKey, oauth2, http-basic, jwt, hmac, mtls, other) are documented on the provided pages.\ndocs: https://obligationsign.com/docs/quickstart/\n"
source_yaml_url: https://artifacts.apis.io/obligationsign-com/authentication/obligationsign-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Governance
- Security
- Infrastructure
---
