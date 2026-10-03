---
anonymous_access: false
api_key_in: []
api_specs:
- filename: noms-brands-api-openapi.yml
  format: yaml
  label: Noms Brands API
  slug: noms-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-brands-api-openapi.yml
- filename: noms-foodgroups-api-openapi.yml
  format: yaml
  label: Noms Food Groups API
  slug: noms-foodgroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-foodgroups-api-openapi.yml
- filename: noms-foods-api-openapi.yml
  format: yaml
  label: Noms Foods API
  slug: noms-foods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-foods-api-openapi.yml
- filename: noms-market-api-openapi.yml
  format: yaml
  label: Noms Market API
  slug: noms-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-market-api-openapi.yml
- filename: noms-nutrients-api-openapi.yml
  format: yaml
  label: Noms Nutrients API
  slug: noms-nutrients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-nutrients-api-openapi.yml
- filename: noms-usage-api-openapi.yml
  format: yaml
  label: Noms Usage API
  slug: noms-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/openapi/noms-usage-api-openapi.yml
auth_types: []
description: Authentication & API keys
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Noms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Noms declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Noms
provider_slug: noms
scheme_count: 2
schemes:
- evidence: 'Send your key in the `X-API-Key` header on every request:'
  header: X-API-Key
  how_to_obtain: Sign up at https://noms.sh/signup, verify your email, then mint a key from your dashboard (Dashboard → API Keys → Create key).
  location: header
  name: API Key
  type: apiKey
- evidence: '`Authorization: Bearer <key>` is accepted and behaves identically to `X-API-Key`.'
  header: Authorization
  how_to_obtain: Sign up at https://noms.sh/signup, verify your email, then mint a key from your dashboard (Dashboard → API Keys → Create key).
  location: header
  name: Bearer Token
  type: http-bearer
slug: noms-authentication
source_filename: noms-authentication.yml
source_heading: Authentication Profile
source_url: https://noms.sh/docs/authentication.md
source_yaml: "generated: '2026-09-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://noms.sh/docs/authentication.md\nsources:\n- https://noms.sh/docs/authentication.md\n- https://noms.sh/docs/authentication\n- https://noms.sh/docs/quickstart.md\n- https://noms.sh/docs/quickstart\ndescription: Authentication & API keys\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Send your key in the `X-API-Key` header on every request:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Sign up at https://noms.sh/signup, verify your email, then mint a key from your dashboard (Dashboard → API Keys → Create key).\n- type: http-bearer\n  name: Bearer Token\n  evidence: '`Authorization: Bearer <key>` is accepted and behaves identically to `X-API-Key`.'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up at https://noms.sh/signup, verify your email, then mint a key from your dashboard (Dashboard → API Keys → Create key).\ndocs: https://noms.sh/docs/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/noms/refs/heads/main/authentication/noms-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Nutrition
- Food
- Data
- Health
---
