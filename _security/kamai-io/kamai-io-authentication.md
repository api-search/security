---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kamai-io-blueprints-actions-api-openapi.yml
  format: yaml
  label: Kamai Blueprints / Actions API
  slug: kamai-io-blueprints-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kamai-io/openapi/kamai-io-blueprints-actions-api-openapi.yml
- filename: kamai-io-blueprints-api-openapi.yml
  format: yaml
  label: Kamai Blueprints API
  slug: kamai-io-blueprints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kamai-io/openapi/kamai-io-blueprints-api-openapi.yml
- filename: kamai-io-blueprints-drawing-text-api-openapi.yml
  format: yaml
  label: Kamai Blueprints / Drawing text API
  slug: kamai-io-blueprints-drawing-text-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kamai-io/openapi/kamai-io-blueprints-drawing-text-api-openapi.yml
- filename: kamai-io-blueprints-files-api-openapi.yml
  format: yaml
  label: Kamai Blueprints / Files API
  slug: kamai-io-blueprints-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kamai-io/openapi/kamai-io-blueprints-files-api-openapi.yml
- filename: kamai-io-blueprints-markups-api-openapi.yml
  format: yaml
  label: Kamai Blueprints / Markups API
  slug: kamai-io-blueprints-markups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kamai-io/openapi/kamai-io-blueprints-markups-api-openapi.yml
- filename: kamai-io-conversations-api-openapi.yml
  format: yaml
  label: Kamai Conversations API
  slug: kamai-io-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kamai-io/openapi/kamai-io-conversations-api-openapi.yml
- filename: kamai-io-messages-api-openapi.yml
  format: yaml
  label: Kamai Messages API
  slug: kamai-io-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kamai-io/openapi/kamai-io-messages-api-openapi.yml
- filename: kamai-io-projects-api-openapi.yml
  format: yaml
  label: Kamai Projects API
  slug: kamai-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kamai-io/openapi/kamai-io-projects-api-openapi.yml
- filename: kamai-io-projects-jobs-api-openapi.yml
  format: yaml
  label: Kamai Projects / Jobs API
  slug: kamai-io-projects-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kamai-io/openapi/kamai-io-projects-jobs-api-openapi.yml
- filename: kamai-io-turns-api-openapi.yml
  format: yaml
  label: Kamai Turns API
  slug: kamai-io-turns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kamai-io/openapi/kamai-io-turns-api-openapi.yml
auth_types: []
description: Authentication schemes for Kamai API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kamai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kamai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kamai
provider_slug: kamai-io
scheme_count: 1
schemes:
- evidence: 'The API uses a static API-key bearer token. Get a key from the Kamai Console at https://admin.kamai.io (sign in, create an API key). Send it on every request:


    Authorization: Bearer <YOUR_API_KEY>'
  header: Authorization
  how_to_obtain: Get a key from the Kamai Console at https://admin.kamai.io (sign in, create an API key).
  location: header
  name: Bearer
  type: http-bearer
slug: kamai-io-authentication
source_filename: kamai-io-authentication.yml
source_heading: Authentication Profile
source_url: https://kamai.io/developers/quickstart.md
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kamai.io/developers/quickstart.md\nsources:\n- https://kamai.io/developers/quickstart.md\n- https://kamai.io/developers/api\ndescription: Authentication schemes for Kamai API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'The API uses a static API-key bearer token. Get a key from the Kamai Console at https://admin.kamai.io (sign in, create an API key).\n    Send it on every request:\n\n\n    Authorization: Bearer <YOUR_API_KEY>'\n  location: header\n  header: Authorization\n  how_to_obtain: Get a key from the Kamai Console at https://admin.kamai.io (sign in, create an API key).\nnote: No OAuth flows are described on the pages.\ndocs: https://kamai.io/developers/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/kamai-io/authentication/kamai-io-authentication.yml
summary_line: 1 scheme
tags:
- Construction
- Artificial Intelligence
- Blueprint Extraction
- Takeoff
- Estimation
- RFI extraction
- Submittal review
- Spec review
---
