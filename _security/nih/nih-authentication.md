---
api_key_in:
- header
- query
api_specs:
- filename: nih-biosample-api-openapi.yml
  format: yaml
  label: National Institutes of Health (NIH) BioSample API
  slug: nih-biosample-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nih/refs/heads/main/openapi/nih-biosample-api-openapi.yml
- filename: nih-gene-api-openapi.yml
  format: yaml
  label: National Institutes of Health (NIH) Gene API
  slug: nih-gene-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nih/refs/heads/main/openapi/nih-gene-api-openapi.yml
- filename: nih-genome-api-openapi.yml
  format: yaml
  label: National Institutes of Health (NIH) Genome API
  slug: nih-genome-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nih/refs/heads/main/openapi/nih-genome-api-openapi.yml
- filename: nih-organelle-api-openapi.yml
  format: yaml
  label: National Institutes of Health (NIH) Organelle API
  slug: nih-organelle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nih/refs/heads/main/openapi/nih-organelle-api-openapi.yml
- filename: nih-prokaryote-api-openapi.yml
  format: yaml
  label: National Institutes of Health (NIH) Prokaryote API
  slug: nih-prokaryote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nih/refs/heads/main/openapi/nih-prokaryote-api-openapi.yml
- filename: nih-stats-api-openapi.yml
  format: yaml
  label: National Institutes of Health (NIH) Stats API
  slug: nih-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nih/refs/heads/main/openapi/nih-stats-api-openapi.yml
- filename: nih-studies-api-openapi.yml
  format: yaml
  label: National Institutes of Health (NIH) Studies API
  slug: nih-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nih/refs/heads/main/openapi/nih-studies-api-openapi.yml
- filename: nih-taxonomy-api-openapi.yml
  format: yaml
  label: National Institutes of Health (NIH) Taxonomy API
  slug: nih-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nih/refs/heads/main/openapi/nih-taxonomy-api-openapi.yml
- filename: nih-version-api-openapi.yml
  format: yaml
  label: National Institutes of Health (NIH) Version API
  slug: nih-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nih/refs/heads/main/openapi/nih-version-api-openapi.yml
- filename: nih-virus-api-openapi.yml
  format: yaml
  label: National Institutes of Health (NIH) Virus API
  slug: nih-virus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nih/refs/heads/main/openapi/nih-virus-api-openapi.yml
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
