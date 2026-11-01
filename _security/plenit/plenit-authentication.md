---
anonymous_access: false
api_key_in: []
api_specs:
- filename: plenit-openapi-generated.yml
  format: yaml
  label: Plenit API
  slug: plenit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/plenit/openapi/_ae-authored/plenit-openapi-generated.yml
auth_types: []
description: Authentication methods published for Plenit.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Plenit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Plenit declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Plenit
provider_slug: plenit
scheme_count: 1
schemes:
- evidence: 'Cada petición a la API lleva el token en la cabecera `Authorization`:'
  header: Authorization
  location: header
  name: API Token
  type: http-bearer
slug: plenit-authentication
source_filename: plenit-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.plenit.com/productos/object-storage/concepts/s3-access-users-and-credentials.md
source_yaml: "generated: '2026-10-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.plenit.com/productos/object-storage/concepts/s3-access-users-and-credentials.md\nsources:\n- https://docs.plenit.com/productos/object-storage/concepts/s3-access-users-and-credentials.md\n- https://docs.plenit.com/productos/object-storage/details/credentials-and-s3-access.md\n- https://docs.plenit.com/referencia/api-tokens.md\n- https://docs.plenit.com/referencia/api-tokens/what-is-an-api-token.md\ndescription: Authentication methods published for Plenit.\nschemes:\n- type: http-bearer\n  name: API Token\n  evidence: 'Cada petición a la API lleva el token en la cabecera `Authorization`:'\n  location: header\n  header: Authorization\ndocs: https://docs.plenit.com/productos/object-storage/concepts/s3-access-users-and-credentials.md\n"
source_yaml_url: https://artifacts.apis.io/plenit/authentication/plenit-authentication.yml
summary_line: 1 scheme
tags:
- Company
- IT
- Platform
- Cloud
- MSP
---
