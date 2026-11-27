---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datosia-net-openapi-generated.yml
  format: yaml
  label: DatosIA API
  slug: datosia-net-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datosia-net/openapi/_ae-authored/datosia-net-openapi-generated.yml
auth_types: []
description: DatosIA authentication uses API keys.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: DatosIA Authentication
name_suffix: Authentication
oauth_flows: []
overview: DatosIA declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DatosIA
provider_slug: datosia-net
scheme_count: 2
schemes:
- evidence: 'Usa una clave por app o entorno. Envíala como x-api-key o Authorization: Bearer .'
  header: x-api-key
  how_to_obtain: Create a key in the account page under "Claves API".
  location: header
  name: x-api-key
  type: apiKey
- evidence: 'Usa una clave por app o entorno. Envíala como x-api-key o Authorization: Bearer .'
  header: Authorization
  how_to_obtain: Create a key in the account page under "Claves API".
  location: header
  name: Authorization
  type: http-bearer
slug: datosia-net-authentication
source_filename: datosia-net-authentication.yml
source_heading: Authentication Profile
source_url: https://datosia.net/account
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://datosia.net/account\nsources:\n- https://datosia.net/account\ndescription: DatosIA authentication uses API keys.\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: 'Usa una clave por app o entorno. Envíala como x-api-key o Authorization: Bearer .'\n  location: header\n  header: x-api-key\n  how_to_obtain: Create a key in the account page under \"Claves API\".\n- type: http-bearer\n  name: Authorization\n  evidence: 'Usa una clave por app o entorno. Envíala como x-api-key o Authorization: Bearer .'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the account page under \"Claves API\".\ndocs: https://datosia.net/account\n"
source_yaml_url: https://artifacts.apis.io/datosia-net/authentication/datosia-net-authentication.yml
summary_line: 2 schemes
tags:
- Data
- Central America
- Open Data
- Statistics
---
