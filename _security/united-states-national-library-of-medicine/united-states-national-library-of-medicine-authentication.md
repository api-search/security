---
api_key_in:
- query
api_specs:
- filename: ncbi-e-utilities-openapi.yml
  format: yaml
  label: NCBI E-Utilities API
  slug: ncbi-e-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/ncbi-e-utilities-openapi.yml
- filename: openapi3.docs.yaml
  format: yaml
  label: NCBI Datasets REST API
  slug: ncbi-datasets-api
  spec_type: OpenAPI
  url: https://www.ncbi.nlm.nih.gov/datasets/docs/v2/openapi3/openapi3.docs.yaml
- filename: ncbi-blast-openapi.yml
  format: yaml
  label: NCBI BLAST URL API
  slug: ncbi-blast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/ncbi-blast-openapi.yml
- filename: nlm-clinicaltrials-openapi.yml
  format: yaml
  label: ClinicalTrials.gov API
  slug: nlm-clinical-trials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-states-national-library-of-medicine/refs/heads/main/openapi/nlm-clinicaltrials-openapi.yml
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
