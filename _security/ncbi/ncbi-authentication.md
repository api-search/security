---
api_key_in:
- header
- query
api_specs:
- filename: ncbi-biosample-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) BioSample API
  slug: ncbi-biosample-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-biosample-api-openapi.yml
- filename: ncbi-gene-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) Gene API
  slug: ncbi-gene-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-gene-api-openapi.yml
- filename: ncbi-genome-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) Genome API
  slug: ncbi-genome-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-genome-api-openapi.yml
- filename: ncbi-organelle-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) Organelle API
  slug: ncbi-organelle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-organelle-api-openapi.yml
- filename: ncbi-prokaryote-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) Prokaryote API
  slug: ncbi-prokaryote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-prokaryote-api-openapi.yml
- filename: ncbi-taxonomy-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) Taxonomy API
  slug: ncbi-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-taxonomy-api-openapi.yml
- filename: ncbi-version-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) Version API
  slug: ncbi-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-version-api-openapi.yml
- filename: ncbi-virus-api-openapi.yml
  format: yaml
  label: National Center for Biotechnology Information (NCBI) Virus API
  slug: ncbi-virus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/openapi/ncbi-virus-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Ncbi Authentication
name_suffix: Authentication
oauth_flows: []
overview: National Center for Biotechnology Information (NCBI) secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: National Center for Biotechnology Information (NCBI)
provider_slug: ncbi
scheme_count: 2
schemes:
- in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/ncbi-datasets-api.yaml
  type: apiKey
- in: header
  name: ApiKeyAuthHeader
  parameter: api-key
  sources:
  - openapi/ncbi-datasets-api.yaml
  type: apiKey
slug: ncbi-authentication
source_filename: ncbi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ncbi-datasets-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/ncbi-datasets-api.yaml\n- name: ApiKeyAuthHeader\n  type: apiKey\n  in: header\n  parameter: api-key\n  sources:\n  - openapi/ncbi-datasets-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ncbi/refs/heads/main/authentication/ncbi-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Bioinformatics
- Genomics
- Life Sciences
- PubMed
- Sequences
- BLAST
- Taxonomy
- Chemistry
- Open Access
---
