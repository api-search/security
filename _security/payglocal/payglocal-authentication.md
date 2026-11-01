---
anonymous_access: false
api_key_in: []
api_specs:
- filename: payglocal-openapi-generated.yml
  format: yaml
  label: PayGlocal API
  slug: payglocal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payglocal/openapi/_ae-authored/payglocal-openapi-generated.yml
auth_types: []
description: Authentication schemes for PayGlocal APIs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Payglocal Authentication
name_suffix: Authentication
oauth_flows: []
overview: PayGlocal declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: PayGlocal
provider_slug: payglocal
scheme_count: 1
schemes:
- evidence: Every request is signed with HmacSHA256 and sent via x-gl-auth + x-gl-digest headers.
  header: x-gl-auth
  how_to_obtain: Static API Key generated from the PayGlocal Partner Dashboard; API Secret used as HMAC signing key.
  location: header
  name: Partner Onboarding HMAC
  type: other
slug: payglocal-authentication
source_filename: payglocal-authentication.yml
source_heading: Authentication Profile
source_url: https://payglocal.in/docs/authentication
source_yaml: "generated: '2026-10-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://payglocal.in/docs/authentication\nsources:\n- https://payglocal.in/docs/authentication\n- https://payglocal.in/docs/api-reference/update-auth-signatory\n- https://payglocal.in/docs/api-reference/payments-v2/paydirect/auth-capture-authorise\n- https://payglocal.in/docs/api-reference/payments-v2/paycollect/auth-capture-authorise\ndescription: Authentication schemes for PayGlocal APIs\nschemes:\n- type: other\n  name: Partner Onboarding HMAC\n  evidence: Every request is signed with HmacSHA256 and sent via x-gl-auth + x-gl-digest headers.\n  location: header\n  header: x-gl-auth\n  how_to_obtain: Static API Key generated from the PayGlocal Partner Dashboard; API Secret used as HMAC signing key.\ndocs: https://payglocal.in/docs/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/payglocal/authentication/payglocal-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Payments
- FinTech
- Cross-Border
- RBI-Authorized
---
