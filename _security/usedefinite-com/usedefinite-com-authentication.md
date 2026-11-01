---
anonymous_access: false
api_key_in: []
api_specs:
- filename: usedefinite-com-openapi-generated.yml
  format: yaml
  label: Definite API
  slug: usedefinite-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usedefinite-com/openapi/_ae-authored/usedefinite-com-openapi-generated.yml
auth_types: []
description: Definite uses tenant API keys for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Usedefinite Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Definite declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Definite
provider_slug: usedefinite-com
scheme_count: 1
schemes:
- evidence: Tenant API keys authenticate REST and SDK access via X-Vault-API-Key .
  header: X-Vault-API-Key
  how_to_obtain: Create a tenant API key from Settings → API Keys; the raw key is shown once at creation.
  location: header
  name: X-Vault-API-Key
  type: apiKey
slug: usedefinite-com-authentication
source_filename: usedefinite-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.usedefinite.com/security/cryptography-and-tokens
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.usedefinite.com/security/cryptography-and-tokens\nsources:\n- https://docs.usedefinite.com/security/cryptography-and-tokens\n- https://docs.usedefinite.com/getting-started\n- https://docs.usedefinite.com/getting-started/verification-runs\ndescription: Definite uses tenant API keys for authentication.\nschemes:\n- type: apiKey\n  name: X-Vault-API-Key\n  evidence: Tenant API keys authenticate REST and SDK access via X-Vault-API-Key .\n  location: header\n  header: X-Vault-API-Key\n  how_to_obtain: Create a tenant API key from Settings → API Keys; the raw key is shown once at creation.\ndocs: https://docs.usedefinite.com/security/cryptography-and-tokens\n"
source_yaml_url: https://artifacts.apis.io/usedefinite-com/authentication/usedefinite-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Finance
- Ontology
- Integration
- SaaS
---
