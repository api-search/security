---
api_key_in:
- query
api_specs:
- filename: united-states-national-library-of-medicine-blast-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine BLAST API
  slug: united-states-national-library-of-medicine-blast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-blast-api-openapi.yml
- filename: united-states-national-library-of-medicine-fetch-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Fetch API
  slug: united-states-national-library-of-medicine-fetch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-fetch-api-openapi.yml
- filename: united-states-national-library-of-medicine-gene-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Gene API
  slug: united-states-national-library-of-medicine-gene-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-gene-api-openapi.yml
- filename: united-states-national-library-of-medicine-genome-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Genome API
  slug: united-states-national-library-of-medicine-genome-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-genome-api-openapi.yml
- filename: united-states-national-library-of-medicine-info-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Info API
  slug: united-states-national-library-of-medicine-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-info-api-openapi.yml
- filename: united-states-national-library-of-medicine-link-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Link API
  slug: united-states-national-library-of-medicine-link-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-link-api-openapi.yml
- filename: united-states-national-library-of-medicine-metadata-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Metadata API
  slug: united-states-national-library-of-medicine-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-metadata-api-openapi.yml
- filename: united-states-national-library-of-medicine-search-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Search API
  slug: united-states-national-library-of-medicine-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-search-api-openapi.yml
- filename: united-states-national-library-of-medicine-studies-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Studies API
  slug: united-states-national-library-of-medicine-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-studies-api-openapi.yml
- filename: united-states-national-library-of-medicine-taxonomy-api-openapi.yml
  format: yaml
  label: United States National Library of Medicine Taxonomy API
  slug: united-states-national-library-of-medicine-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/united-states-national-library-of-medicine-taxonomy-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: United States National Library Of Medicine Authentication
name_suffix: Authentication
oauth_flows: []
overview: United States National Library of Medicine secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: United States National Library of Medicine
provider_slug: united-states-national-library-of-medicine
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/ncbi-datasets-openapi.yml
  - openapi/ncbi-e-utilities-openapi.yml
  type: apiKey
slug: united-states-national-library-of-medicine-authentication
source_filename: united-states-national-library-of-medicine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ncbi-datasets-openapi.yml, openapi/ncbi-e-utilities-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/ncbi-datasets-openapi.yml\n  - openapi/ncbi-e-utilities-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/authentication/united-states-national-library-of-medicine-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Federal Government
- Biomedical Research
- Healthcare
- Genomics
- Literature
---
