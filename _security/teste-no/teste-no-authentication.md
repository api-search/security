---
anonymous_access: false
api_key_in: []
api_specs:
- filename: teste-no-openapi-generated.yml
  format: yaml
  label: Teste.no API
  slug: teste-no-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teste-no/openapi/_ae-authored/teste-no-openapi-generated.yml
auth_types: []
description: Authentication schemes for Teste.no
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Teste.no Authentication
name_suffix: Authentication
oauth_flows: []
overview: Teste.no declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Teste.no
provider_slug: teste-no
scheme_count: 1
schemes:
- evidence: Teste.no uses API tokens for programmatic access.
  header: Authorization
  how_to_obtain: Create via Settings → API Keys, click Create API Key, copy the token shown once.
  location: header
  name: API Token
  type: http-bearer
slug: teste-no-authentication
source_filename: teste-no-authentication.yml
source_heading: Authentication Profile
source_url: https://teste.no/docs/api
source_yaml: "generated: '2026-11-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://teste.no/docs/api\nsources:\n- https://teste.no/docs/api\n- https://teste.no/docs/getting-started\ndescription: Authentication schemes for Teste.no\nschemes:\n- type: http-bearer\n  name: API Token\n  evidence: Teste.no uses API tokens for programmatic access.\n  location: header\n  header: Authorization\n  how_to_obtain: Create via Settings → API Keys, click Create API Key, copy the token shown once.\ndocs: https://teste.no/docs/api\n"
source_yaml_url: https://artifacts.apis.io/teste-no/authentication/teste-no-authentication.yml
summary_line: 1 scheme
tags:
- Monitoring
- Testing
- Security
- Performance
- SEO
- Accessibility
- E‑commerce
- API
---
