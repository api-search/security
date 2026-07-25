---
api_key_in:
- query
api_specs:
- filename: pubmed-history-api-openapi.yml
  format: yaml
  label: PubMed History API
  slug: pubmed-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-history-api-openapi.yml
- filename: pubmed-info-api-openapi.yml
  format: yaml
  label: PubMed Info API
  slug: pubmed-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-info-api-openapi.yml
- filename: pubmed-links-api-openapi.yml
  format: yaml
  label: PubMed Links API
  slug: pubmed-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-links-api-openapi.yml
- filename: pubmed-retrieval-api-openapi.yml
  format: yaml
  label: PubMed Retrieval API
  slug: pubmed-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-retrieval-api-openapi.yml
- filename: pubmed-search-api-openapi.yml
  format: yaml
  label: PubMed Search API
  slug: pubmed-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-search-api-openapi.yml
- filename: pubmed-summary-api-openapi.yml
  format: yaml
  label: PubMed Summary API
  slug: pubmed-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/openapi/pubmed-summary-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pubmed Authentication
name_suffix: Authentication
oauth_flows: []
overview: PubMed secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PubMed
provider_slug: pubmed
scheme_count: 1
schemes:
- description: 'Optional NCBI API key. Without a key: 3 requests/second. With a key: 10 requests/second. Register at https://www.ncbi.nlm.nih.gov/account/'
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/entrez-eutils.json
  type: apiKey
slug: pubmed-authentication
source_filename: pubmed-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/entrez-eutils.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: 'Optional NCBI API key. Without a key: 3 requests/second. With a key: 10 requests/second.\n    Register at https://www.ncbi.nlm.nih.gov/account/'\n  sources:\n  - openapi/entrez-eutils.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pubmed/refs/heads/main/authentication/pubmed-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- biomedical
- life science
- research
- literature
- citations
- abstracts
- MeSH
- genomics
- PubMed
- NCBI
---
