---
anonymous_access: false
api_key_in: []
api_specs:
- filename: medsender-ai-documents-api-openapi.yml
  format: yaml
  label: Medsender AI Documents API
  slug: medsender-ai-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-ai-documents-api-openapi.yml
- filename: medsender-clients-api-openapi.yml
  format: yaml
  label: Medsender Clients API
  slug: medsender-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-clients-api-openapi.yml
- filename: medsender-fax-numbers-api-openapi.yml
  format: yaml
  label: Medsender Fax Numbers API
  slug: medsender-fax-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-fax-numbers-api-openapi.yml
- filename: medsender-received-faxes-api-openapi.yml
  format: yaml
  label: Medsender Received Faxes API
  slug: medsender-received-faxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-received-faxes-api-openapi.yml
- filename: medsender-secure-links-api-openapi.yml
  format: yaml
  label: Medsender Secure Links API
  slug: medsender-secure-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-secure-links-api-openapi.yml
- filename: medsender-sent-faxes-api-openapi.yml
  format: yaml
  label: Medsender Sent Faxes API
  slug: medsender-sent-faxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-sent-faxes-api-openapi.yml
- filename: medsender-v3-fax-numbers-api-openapi.yml
  format: yaml
  label: Medsender V3 Fax Numbers API
  slug: medsender-v3-fax-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-v3-fax-numbers-api-openapi.yml
- filename: medsender-v3-received-faxes-api-openapi.yml
  format: yaml
  label: Medsender V3 Received Faxes API
  slug: medsender-v3-received-faxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-v3-received-faxes-api-openapi.yml
- filename: medsender-v3-sent-faxes-api-openapi.yml
  format: yaml
  label: Medsender V3 Sent Faxes API
  slug: medsender-v3-sent-faxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/medsender/openapi/medsender-v3-sent-faxes-api-openapi.yml
auth_types: []
description: Authentication uses a self‑contained API key with the Bearer scheme sent in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Medsender Authentication
name_suffix: Authentication
oauth_flows: []
overview: Medsender declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Medsender
provider_slug: medsender
scheme_count: 1
schemes:
- evidence: Use a self-contained API key with the Bearer scheme.
  header: Authorization
  how_to_obtain: Through self‑serve activation (email verification, BAA, number selection, and a card) or coordinated enterprise enrollment; test keys start with `sk_test_`, live keys start with `sk_live_`.
  location: header
  name: Bearer
  type: http-bearer
slug: medsender-authentication
source_filename: medsender-authentication.yml
source_heading: Authentication Profile
source_url: https://developer.medsender.com/docs/authentication.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developer.medsender.com/docs/authentication.md\nsources:\n- https://developer.medsender.com/docs/authentication.md\n- https://developer.medsender.com/docs/authentication\n- https://developer.medsender.com/docs/legacy\ndescription: Authentication uses a self‑contained API key with the Bearer scheme sent in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Use a self-contained API key with the Bearer scheme.\n  location: header\n  header: Authorization\n  how_to_obtain: Through self‑serve activation (email verification, BAA, number selection, and a card) or coordinated enterprise enrollment; test\n    keys start with `sk_test_`, live keys start with `sk_live_`.\nnote: No OAuth2 flows, API‑key query or body parameters, or other authentication schemes are documented.\ndocs: https://developer.medsender.com/docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/medsender/authentication/medsender-authentication.yml
summary_line: 1 scheme
tags:
- Referral Management
- Fax Automation
- Patient Recapture
- Call Automation
- EHR Integration
---
