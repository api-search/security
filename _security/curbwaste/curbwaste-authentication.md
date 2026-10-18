---
anonymous_access: false
api_key_in: []
api_specs:
- filename: curbwaste-catalog-api-openapi.yml
  format: yaml
  label: Curbwaste Catalog API
  slug: curbwaste-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curbwaste/refs/heads/main/openapi/curbwaste-catalog-api-openapi.yml
- filename: curbwaste-customers-api-openapi.yml
  format: yaml
  label: Curbwaste Customers API
  slug: curbwaste-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curbwaste/refs/heads/main/openapi/curbwaste-customers-api-openapi.yml
- filename: curbwaste-locations-api-openapi.yml
  format: yaml
  label: Curbwaste Locations API
  slug: curbwaste-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curbwaste/refs/heads/main/openapi/curbwaste-locations-api-openapi.yml
- filename: curbwaste-zones-api-openapi.yml
  format: yaml
  label: Curbwaste Zones API
  slug: curbwaste-zones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/curbwaste/refs/heads/main/openapi/curbwaste-zones-api-openapi.yml
auth_types: []
description: CurbWaste authenticates partner API requests with company API keys passed as Bearer tokens in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Curbwaste Authentication
name_suffix: Authentication
oauth_flows: []
overview: Curbwaste declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Curbwaste
provider_slug: curbwaste
scheme_count: 1
schemes:
- evidence: CurbWaste authenticates **partner** API requests with company API keys passed as Bearer tokens. Every request to `/v1/*` must include a valid key in the `Authorization` header.
  header: Authorization
  how_to_obtain: Create an API key in the Developer Platform (https://platform.curbwaste.com) under **API Keys**, then copy the `cw_live_…` secret.
  location: header
  name: Bearer
  scopes:
  - customers:read
  - customers:write
  type: http-bearer
slug: curbwaste-authentication
source_filename: curbwaste-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.curbwaste.com/authentication.md
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.curbwaste.com/authentication.md\nsources:\n- https://docs.curbwaste.com/authentication.md\n- https://docs.curbwaste.com/quickstart.md\n- https://docs.curbwaste.com/guides/webhooks-setup.md\ndescription: CurbWaste authenticates partner API requests with company API keys passed as Bearer tokens in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: CurbWaste authenticates **partner** API requests with company API keys passed as Bearer tokens. Every request to `/v1/*` must include\n    a valid key in the `Authorization` header.\n  location: header\n  header: Authorization\n  scopes:\n  - customers:read\n  - customers:write\n  how_to_obtain: Create an API key in the Developer Platform (https://platform.curbwaste.com) under **API Keys**, then copy the `cw_live_…` secret.\nnote: No OAuth2, API key query, or other authentication schemes are\
  \ documented.\ndocs: https://docs.curbwaste.com/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curbwaste/refs/heads/main/authentication/curbwaste-authentication.yml
summary_line: 1 scheme
tags:
- Waste
- Software
- Software-as-a-Service
- Logistics
- Haulers
---
