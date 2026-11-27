---
anonymous_access: false
api_key_in: []
api_specs:
- filename: consequential-io-openapi-generated.yml
  format: yaml
  label: Consequential API
  slug: consequential-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/consequential-io/openapi/_ae-authored/consequential-io-openapi-generated.yml
auth_types: []
description: Authentication methods for Consequential API as described on the page.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Consequential Authentication
name_suffix: Authentication
oauth_flows: []
overview: Consequential declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Consequential
provider_slug: consequential-io
scheme_count: 3
schemes:
- evidence: Auth Request a magic sign-in link (rate-limited) POST
  header: Authorization
  how_to_obtain: Request a magic sign-in link via the Auth endpoint, then exchange the link for an access token.
  location: header
  name: Magic Link
  type: http-bearer
- evidence: Begin Google OAuth sign-in (redirect) GET
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Start the Google OAuth sign‑in flow, receive an authorization code, and exchange it for a token.
  location: header
  name: Google OAuth
  type: oauth2
- evidence: Verify a JWT and return its claims (inter-service use) POST
  header: Authorization
  how_to_obtain: Provide a JWT to the verification endpoint to obtain its claims.
  location: header
  name: JWT Verification
  type: http-bearer
slug: consequential-io-authentication
source_filename: consequential-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.consequential.io/guides/send-your-first-request/
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.consequential.io/guides/send-your-first-request/\nsources:\n- https://docs.consequential.io/guides/send-your-first-request/\ndescription: Authentication methods for Consequential API as described on the page.\nschemes:\n- type: http-bearer\n  name: Magic Link\n  evidence: Auth Request a magic sign-in link (rate-limited) POST\n  location: header\n  header: Authorization\n  how_to_obtain: Request a magic sign-in link via the Auth endpoint, then exchange the link for an access token.\n- type: oauth2\n  name: Google OAuth\n  evidence: Begin Google OAuth sign-in (redirect) GET\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  how_to_obtain: Start the Google OAuth sign‑in flow, receive an authorization code, and exchange it for a token.\n- type: http-bearer\n  name: JWT Verification\n  evidence: Verify a JWT and return its claims (inter-service\
  \ use) POST\n  location: header\n  header: Authorization\n  how_to_obtain: Provide a JWT to the verification endpoint to obtain its claims.\ndocs: https://docs.consequential.io/guides/send-your-first-request/\n"
source_yaml_url: https://artifacts.apis.io/consequential-io/authentication/consequential-io-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Advertising
- E-Commerce
- Revenue Intelligence
- Software-as-a-Service
---
