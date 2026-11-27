---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: zornade-com Authentication
name_suffix: Authentication
oauth_flows: []
overview: zornade-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: zornade-com
provider_slug: zornade-com
scheme_count: 1
schemes:
- evidence: Tutti gli endpoint richiedono un token API in header x-api-key , tranne /health .
  header: x-api-key
  how_to_obtain: Crea un account per generare token API personali.
  location: header
  name: x-api-key
  scopes:
  - geocoding:read
  - admin_data:read
  - parcels:read
  type: apiKey
slug: zornade-com-authentication
source_filename: zornade-com-authentication.yml
source_heading: Authentication Profile
source_url: https://app.zornade.com/api/
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://app.zornade.com/api/\nsources:\n- https://app.zornade.com/api/\n- https://app.zornade.com/auth\ndescription: Authentication\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: Tutti gli endpoint richiedono un token API in header x-api-key , tranne /health .\n  location: header\n  header: x-api-key\n  scopes:\n  - geocoding:read\n  - admin_data:read\n  - parcels:read\n  how_to_obtain: Crea un account per generare token API personali.\nnote: No OAuth2, HTTP Bearer, or other authentication schemes are documented.\ndocs: https://app.zornade.com/api/\n"
source_yaml_url: https://artifacts.apis.io/zornade-com/authentication/zornade-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data
- GIS
- Italy
- Land Registry
---
