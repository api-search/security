---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fabrica-land-change-of-ownership-api-openapi.yml
  format: yaml
  label: fabrica-land Change Of Ownership API
  slug: fabrica-land-change-of-ownership-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-change-of-ownership-api-openapi.yml
- filename: fabrica-land-document-api-openapi.yml
  format: yaml
  label: fabrica-land Document API
  slug: fabrica-land-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-document-api-openapi.yml
- filename: fabrica-land-media-api-openapi.yml
  format: yaml
  label: fabrica-land Media API
  slug: fabrica-land-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-media-api-openapi.yml
- filename: fabrica-land-metadata-api-openapi.yml
  format: yaml
  label: fabrica-land Metadata API
  slug: fabrica-land-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-metadata-api-openapi.yml
- filename: fabrica-land-off-ramp-api-openapi.yml
  format: yaml
  label: fabrica-land Off Ramp API
  slug: fabrica-land-off-ramp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-off-ramp-api-openapi.yml
- filename: fabrica-land-on-ramp-api-openapi.yml
  format: yaml
  label: fabrica-land On Ramp API
  slug: fabrica-land-on-ramp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-on-ramp-api-openapi.yml
- filename: fabrica-land-pool-lending-api-openapi.yml
  format: yaml
  label: fabrica-land Pool Lending API
  slug: fabrica-land-pool-lending-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-pool-lending-api-openapi.yml
- filename: fabrica-land-proof-of-ownership-api-openapi.yml
  format: yaml
  label: fabrica-land Proof Of Ownership API
  slug: fabrica-land-proof-of-ownership-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-proof-of-ownership-api-openapi.yml
- filename: fabrica-land-regrid-api-openapi.yml
  format: yaml
  label: fabrica-land Regrid API
  slug: fabrica-land-regrid-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-regrid-api-openapi.yml
- filename: fabrica-land-syndication-api-openapi.yml
  format: yaml
  label: fabrica-land Syndication API
  slug: fabrica-land-syndication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-syndication-api-openapi.yml
- filename: fabrica-land-terrain-project-api-openapi.yml
  format: yaml
  label: fabrica-land Terrain Project API
  slug: fabrica-land-terrain-project-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-terrain-project-api-openapi.yml
- filename: fabrica-land-token-api-openapi.yml
  format: yaml
  label: fabrica-land Token API
  slug: fabrica-land-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-token-api-openapi.yml
- filename: fabrica-land-valuation-api-openapi.yml
  format: yaml
  label: fabrica-land Valuation API
  slug: fabrica-land-valuation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabrica-land/openapi/fabrica-land-valuation-api-openapi.yml
auth_types: []
description: Authentication schemes as published on Fabrica Land API documentation pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Fabrica Land Authentication
name_suffix: Authentication
oauth_flows: []
overview: fabrica-land declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: fabrica-land
provider_slug: fabrica-land
scheme_count: 2
schemes:
- evidence: Credentials Bearer
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
- evidence: Credentials Bearer jwt
  header: Authorization
  location: header
  name: Bearer JWT
  type: jwt
slug: fabrica-land-authentication
source_filename: fabrica-land-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.fabrica.land/docs/token-recovery.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.fabrica.land/docs/token-recovery.md\nsources:\n- https://docs.fabrica.land/docs/token-recovery.md\n- https://docs.fabrica.land/docs/property-nft.md\n- https://docs.fabrica.land/reference/getonramps\n- https://docs.fabrica.land/reference/markonrampcelebrationcomplete\ndescription: Authentication schemes as published on Fabrica Land API documentation pages.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Credentials Bearer\n  location: header\n  header: Authorization\n- type: jwt\n  name: Bearer JWT\n  evidence: Credentials Bearer jwt\n  location: header\n  header: Authorization\ndocs: https://docs.fabrica.land/docs/token-recovery.md\n"
source_yaml_url: https://artifacts.apis.io/fabrica-land/authentication/fabrica-land-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Real Estate
- Blockchain
- Marketplace
- FinTech
---
