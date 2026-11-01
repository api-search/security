---
anonymous_access: false
api_key_in: []
api_specs:
- filename: finevoice-openapi-generated.yml
  format: yaml
  label: FineVoice (Fineshare) API
  slug: finevoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finevoice/openapi/_ae-authored/finevoice-openapi-generated.yml
- filename: finevoice-openapi-openapi.json
  format: json
  label: FineVoice (Fineshare) Openapi API
  slug: finevoice-fineshare-openapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finevoice/openapi/_original/finevoice-openapi-openapi.json
- filename: finevoice-changeaudiofile-openapi.json
  format: json
  label: FineVoice (Fineshare) Changeaudiofile API
  slug: finevoice-fineshare-changeaudiofile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finevoice/openapi/_original/finevoice-changeaudiofile-openapi.json
- filename: finevoice-listmodels-openapi.json
  format: json
  label: FineVoice (Fineshare) Listmodels API
  slug: finevoice-fineshare-listmodels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finevoice/openapi/_original/finevoice-listmodels-openapi.json
- filename: finevoice-pagevoices-openapi.json
  format: json
  label: FineVoice (Fineshare) Pagevoices API
  slug: finevoice-fineshare-pagevoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finevoice/openapi/_original/finevoice-pagevoices-openapi.json
- filename: finevoice-getvoicedetail-openapi.json
  format: json
  label: FineVoice (Fineshare) Getvoicedetail API
  slug: finevoice-fineshare-getvoicedetail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finevoice/openapi/_original/finevoice-getvoicedetail-openapi.json
- filename: finevoice-uploadaudiofile-openapi.json
  format: json
  label: FineVoice (Fineshare) Uploadaudiofile API
  slug: finevoice-fineshare-uploadaudiofile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finevoice/openapi/_original/finevoice-uploadaudiofile-openapi.json
- filename: finevoice-createaudiofilechanger-openapi.json
  format: json
  label: FineVoice (Fineshare) Createaudiofilechanger API
  slug: finevoice-fineshare-createaudiofilechanger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finevoice/openapi/_original/finevoice-createaudiofilechanger-openapi.json
auth_types: []
description: Authentication uses an API key passed as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Finevoice Authentication
name_suffix: Authentication
oauth_flows: []
overview: FineVoice (Fineshare) declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: FineVoice (Fineshare)
provider_slug: finevoice
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer $FINEVOICE_API_KEY'
  header: Authorization
  how_to_obtain: Generate the API key in the FineVoice User Center under API Tokens.
  location: header
  name: Bearer
  type: http-bearer
slug: finevoice-authentication
source_filename: finevoice-authentication.yml
source_heading: Authentication Profile
source_url: https://api.finevoice.ai/quickstart.md
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.finevoice.ai/quickstart.md\nsources:\n- https://api.finevoice.ai/quickstart.md\ndescription: Authentication uses an API key passed as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authorization: Bearer $FINEVOICE_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate the API key in the FineVoice User Center under API Tokens.\ndocs: https://api.finevoice.ai/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/finevoice/authentication/finevoice-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Voice
- Text-to-Speech
- Audio
---
