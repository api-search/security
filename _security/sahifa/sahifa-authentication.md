---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sahifa-convert-api-openapi.yml
  format: yaml
  label: Sahifa Convert API
  slug: sahifa-convert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sahifa/refs/heads/main/openapi/sahifa-convert-api-openapi.yml
- filename: sahifa-health-api-openapi.yml
  format: yaml
  label: Sahifa Health API
  slug: sahifa-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sahifa/refs/heads/main/openapi/sahifa-health-api-openapi.yml
- filename: sahifa-take-api-openapi.yml
  format: yaml
  label: Sahifa Take API
  slug: sahifa-take-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sahifa/refs/heads/main/openapi/sahifa-take-api-openapi.yml
auth_types: []
description: Authentication methods for Sahifa API
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Sahifa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sahifa declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Sahifa
provider_slug: sahifa
scheme_count: 5
schemes:
- evidence: 'X-API-Key header X-API-Key: sk_live_... Any client'
  header: X-API-Key
  how_to_obtain: From the Sahifa dashboard; the key is provided after signing up.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'X-Access-Key header X-Access-Key: sk_live_... Any client'
  header: X-Access-Key
  how_to_obtain: From the Sahifa dashboard; the key is provided after signing up.
  location: header
  name: X-Access-Key
  type: apiKey
- evidence: access_key query parameter /take?access_key=sk_live_...&url=... ScreenshotOne clients
  how_to_obtain: From the Sahifa dashboard; the key is provided after signing up.
  location: query
  name: access_key
  type: apiKey
- evidence: 'Bearer token Authorization: Bearer sk_live_... Any client'
  header: Authorization
  how_to_obtain: From the Sahifa dashboard; the key is provided after signing up.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: Basic authentication user api , password = your key PDFShift clients
  header: Authorization
  how_to_obtain: Use username "api" and the API key as the password; the key is provided after signing up.
  location: header
  name: Basic authentication
  type: http-basic
slug: sahifa-authentication
source_filename: sahifa-authentication.yml
source_heading: Authentication Profile
source_url: https://sahifa.dev/en/docs/authentication
source_yaml: "generated: '2026-09-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://sahifa.dev/en/docs/authentication\nsources:\n- https://sahifa.dev/en/docs/authentication\n- https://sahifa.dev/en/docs/quickstart\ndescription: Authentication methods for Sahifa API\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'X-API-Key header X-API-Key: sk_live_... Any client'\n  location: header\n  header: X-API-Key\n  how_to_obtain: From the Sahifa dashboard; the key is provided after signing up.\n- type: apiKey\n  name: X-Access-Key\n  evidence: 'X-Access-Key header X-Access-Key: sk_live_... Any client'\n  location: header\n  header: X-Access-Key\n  how_to_obtain: From the Sahifa dashboard; the key is provided after signing up.\n- type: apiKey\n  name: access_key\n  evidence: access_key query parameter /take?access_key=sk_live_...&url=... ScreenshotOne clients\n  location: query\n  how_to_obtain: From the Sahifa dashboard; the key is provided after signing\
  \ up.\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Bearer token Authorization: Bearer sk_live_... Any client'\n  location: header\n  header: Authorization\n  how_to_obtain: From the Sahifa dashboard; the key is provided after signing up.\n- type: http-basic\n  name: Basic authentication\n  evidence: Basic authentication user api , password = your key PDFShift clients\n  location: header\n  header: Authorization\n  how_to_obtain: Use username \"api\" and the API key as the password; the key is provided after signing up.\nnote: No OAuth2 flows are documented for Sahifa.\ndocs: https://sahifa.dev/en/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sahifa/refs/heads/main/authentication/sahifa-authentication.yml
summary_line: 5 schemes
tags:
- Company
- PDF
- Screenshot
- API
- SaudiArabia
- Cloud
---
