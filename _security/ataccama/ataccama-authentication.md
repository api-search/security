---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ataccama-ataccama-api-api-openapi.yml
  format: yaml
  label: Ataccama Ataccama API
  slug: ataccama-ataccama-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ataccama/refs/heads/main/openapi/ataccama-ataccama-api-api-openapi.yml
- filename: ataccama-catalog-api-openapi.yml
  format: yaml
  label: Ataccama Catalog API
  slug: ataccama-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ataccama/refs/heads/main/openapi/ataccama-catalog-api-openapi.yml
- filename: ataccama-data-quality-api-openapi.yml
  format: yaml
  label: Ataccama Data Quality API
  slug: ataccama-data-quality-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ataccama/refs/heads/main/openapi/ataccama-data-quality-api-openapi.yml
- filename: ataccama-reference-data-api-openapi.yml
  format: yaml
  label: Ataccama Reference Data API
  slug: ataccama-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ataccama/refs/heads/main/openapi/ataccama-reference-data-api-openapi.yml
- filename: ataccama-rest-api-openapi.yml
  format: yaml
  label: Ataccama Rest API
  slug: ataccama-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ataccama/refs/heads/main/openapi/ataccama-rest-api-openapi.yml
auth_types: []
description: Authentication for Ataccama ONE APIs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ataccama Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ataccama declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ataccama
provider_slug: ataccama
scheme_count: 1
schemes:
- evidence: The only supported provider of access tokens for ONE is Keycloak.
  flows:
  - client_credentials
  how_to_obtain: Obtain an access token from Keycloak using a service account client with either Client ID and Secret or JSON Web authentication.
  name: Keycloak
  type: oauth2
slug: ataccama-authentication
source_filename: ataccama-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ataccama.com/one/latest/one-apis/api-requests-authentication.html
source_yaml: "generated: '2026-09-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ataccama.com/one/latest/one-apis/api-requests-authentication.html\nsources:\n- https://docs.ataccama.com/one/latest/one-apis/api-requests-authentication.html\n- https://docs.ataccama.com/one/latest/getting-started/get-started-with-data-quality.html\n- https://docs.ataccama.com/one/latest/getting-started/get-started-with-catalog-and-glossary.html\n- https://docs.ataccama.com/one/latest/getting-started/get-started-with-data-observability.html\ndescription: Authentication for Ataccama ONE APIs\nschemes:\n- type: oauth2\n  name: Keycloak\n  evidence: The only supported provider of access tokens for ONE is Keycloak.\n  flows:\n  - client_credentials\n  how_to_obtain: Obtain an access token from Keycloak using a service account client with either Client ID and Secret or JSON Web authentication.\ndocs: https://docs.ataccama.com/one/latest/one-apis/api-requests-authentication.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ataccama/refs/heads/main/authentication/ataccama-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data Quality
- Data Governance
- Artificial Intelligence
- Enterprise
- Platform
---
