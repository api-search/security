---
anonymous_access: false
api_key_in: []
api_specs:
- filename: testchimp-io-openapi-generated.yml
  format: yaml
  label: TestChimp API
  slug: testchimp-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/testchimp-io/openapi/_ae-authored/testchimp-io-openapi-generated.yml
auth_types: []
description: Authentication for Clerk used in TestChimp testing guides.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: TestChimp Authentication
name_suffix: Authentication
oauth_flows: []
overview: TestChimp declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: TestChimp
provider_slug: testchimp-io
scheme_count: 1
schemes:
- evidence: Set CLERK_PUBLISHABLE_KEY , CLERK_SECRET_KEY , and CLERK_TESTING_TOKEN from Clerk testing docs.
  header: Authorization
  location: header
  name: Clerk API Key
  type: http-bearer
slug: testchimp-io-authentication
source_filename: testchimp-io-authentication.yml
source_heading: Authentication Profile
source_url: https://testchimp.io/guides/auth/testing-clerk-auth-playwright/
source_yaml: "generated: '2026-11-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://testchimp.io/guides/auth/testing-clerk-auth-playwright/\nsources:\n- https://testchimp.io/guides/auth/testing-clerk-auth-playwright/\n- https://testchimp.io/guides/auth/testing-firebase-auth/\n- https://testchimp.io/guides/auth/testing-oauth-social-login/\n- https://testchimp.io/docs/release-management/secrets-scan/\ndescription: Authentication for Clerk used in TestChimp testing guides.\nschemes:\n- type: http-bearer\n  name: Clerk API Key\n  evidence: Set CLERK_PUBLISHABLE_KEY , CLERK_SECRET_KEY , and CLERK_TESTING_TOKEN from Clerk testing docs.\n  location: header\n  header: Authorization\ndocs: https://testchimp.io/guides/auth/testing-clerk-auth-playwright/\n"
source_yaml_url: https://artifacts.apis.io/testchimp-io/authentication/testchimp-io-authentication.yml
summary_line: 1 scheme
tags:
- QA
- Release Governance
- Agent‑Driven Testing
---
