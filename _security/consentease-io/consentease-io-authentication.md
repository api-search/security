---
anonymous_access: false
api_key_in: []
api_specs:
- filename: consentease-io-openapi-generated.yml
  format: yaml
  label: ConsentEase API
  slug: consentease-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/consentease-io/openapi/_ae-authored/consentease-io-openapi-generated.yml
auth_types: []
description: Authentication methods for ConsentEase API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ConsentEase Authentication
name_suffix: Authentication
oauth_flows: []
overview: ConsentEase declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ConsentEase
provider_slug: consentease-io
scheme_count: 2
schemes:
- evidence: 'Send either Authorization: Bearer YOUR_API_KEY or X-API-Key: YOUR_API_KEY.'
  header: Authorization
  how_to_obtain: Create an API key in Settings → API Keys and copy the displayed ce_live_… value.
  location: header
  name: Bearer
  type: http-bearer
- evidence: 'Send either Authorization: Bearer YOUR_API_KEY or X-API-Key: YOUR_API_KEY.'
  header: X-API-Key
  how_to_obtain: Create an API key in Settings → API Keys and copy the displayed ce_live_… value.
  location: header
  name: X-API-Key
  type: apiKey
slug: consentease-io-authentication
source_filename: consentease-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.consentease.io/api-keys
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.consentease.io/api-keys\nsources:\n- https://docs.consentease.io/api-keys\n- https://docs.consentease.io/quickstart\ndescription: Authentication methods for ConsentEase API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send either Authorization: Bearer YOUR_API_KEY or X-API-Key: YOUR_API_KEY.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings → API Keys and copy the displayed ce_live_… value.\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Send either Authorization: Bearer YOUR_API_KEY or X-API-Key: YOUR_API_KEY.'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an API key in Settings → API Keys and copy the displayed ce_live_… value.\ndocs: https://docs.consentease.io/api-keys\n"
source_yaml_url: https://artifacts.apis.io/consentease-io/authentication/consentease-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- GDPR
- CCPA
- Cookie Consent
- Small Business
---
