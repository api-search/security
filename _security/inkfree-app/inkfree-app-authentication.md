---
anonymous_access: false
api_key_in: []
api_specs:
- filename: inkfree-app-openapi-generated.yml
  format: yaml
  label: Inkfree API
  slug: inkfree-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inkfree-app/openapi/_ae-authored/inkfree-app-openapi-generated.yml
auth_types: []
description: Inkfree API authenticates with a single API key sent in a request header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Inkfree Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inkfree declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Inkfree
provider_slug: inkfree-app
scheme_count: 1
schemes:
- evidence: 'Every /api/v1/inkfree/** endpoint requires an API key sent in the X-API-Key header:'
  header: X-API-Key
  how_to_obtain: Sign in to Inkfree, open Account Settings → API Keys, and create a key. The full sk_live_... value is displayed once at creation.
  location: header
  name: API Key
  type: apiKey
slug: inkfree-app-authentication
source_filename: inkfree-app-authentication.yml
source_heading: Authentication Profile
source_url: https://inkfree.app/docs/authentication/
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://inkfree.app/docs/authentication/\nsources:\n- https://inkfree.app/docs/authentication/\n- https://inkfree.app/help/security-and-authentication/\n- https://inkfree.app/docs/authentication/\n- https://inkfree.app/features/signing-order/\ndescription: Inkfree API authenticates with a single API key sent in a request header.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Every /api/v1/inkfree/** endpoint requires an API key sent in the X-API-Key header:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Sign in to Inkfree, open Account Settings → API Keys, and create a key. The full sk_live_... value is displayed once at creation.\ndocs: https://inkfree.app/docs/authentication/\n"
source_yaml_url: https://artifacts.apis.io/inkfree-app/authentication/inkfree-app-authentication.yml
summary_line: 1 scheme
tags:
- E-Signature
- Software-as-a-Service
- Cloud
- Document Management
---
