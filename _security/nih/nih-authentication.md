---
api_key_in:
- header
- query
api_specs:
- filename: datasets.openapi.yaml
  format: yaml
  label: NCBI Datasets v2 REST API
  slug: ncbi-datasets-v2-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/ncbi/datasets/master/datasets.openapi.yaml
- filename: v2
  format: yaml
  label: ClinicalTrials.gov REST API
  slug: clinicaltrialsgov-rest-api
  spec_type: OpenAPI
  url: https://clinicaltrials.gov/api/oas/v2
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nih Authentication
name_suffix: Authentication
oauth_flows: []
overview: National Institutes of Health (NIH) secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: National Institutes of Health (NIH)
provider_slug: nih
scheme_count: 2
schemes:
- in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/ncbi-datasets-v2.yaml
  type: apiKey
- in: header
  name: ApiKeyAuthHeader
  parameter: api-key
  sources:
  - openapi/ncbi-datasets-v2.yaml
  type: apiKey
slug: nih-authentication
source_filename: nih-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ncbi-datasets-v2.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/ncbi-datasets-v2.yaml\n- name: ApiKeyAuthHeader\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/ncbi-datasets-v2.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nih/refs/heads/main/authentication/nih-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Biomedical
- Research
- PubMed
- ClinicalTrials
- PubChem
- Genomics
- Health
- Science
- Government
---
