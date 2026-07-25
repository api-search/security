---
api_key_in:
- header
api_specs:
- filename: us-patent-and-trademark-office-bulk-datasets-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office Bulk Datasets API
  slug: us-patent-and-trademark-office-bulk-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-bulk-datasets-api-openapi.yml
- filename: us-patent-and-trademark-office-case-documents-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office Case Documents API
  slug: us-patent-and-trademark-office-case-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-case-documents-api-openapi.yml
- filename: us-patent-and-trademark-office-case-status-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office Case Status API
  slug: us-patent-and-trademark-office-case-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-case-status-api-openapi.yml
- filename: us-patent-and-trademark-office-patent-search-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office Patent Search API
  slug: us-patent-and-trademark-office-patent-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-patent-search-api-openapi.yml
- filename: us-patent-and-trademark-office-petition-decisions-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office Petition Decisions API
  slug: us-patent-and-trademark-office-petition-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-petition-decisions-api-openapi.yml
- filename: us-patent-and-trademark-office-ptab-appeals-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office PTAB Appeals API
  slug: us-patent-and-trademark-office-ptab-appeals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-ptab-appeals-api-openapi.yml
- filename: us-patent-and-trademark-office-ptab-interferences-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office PTAB Interferences API
  slug: us-patent-and-trademark-office-ptab-interferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-ptab-interferences-api-openapi.yml
- filename: us-patent-and-trademark-office-ptab-trials-decisions-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office PTAB Trials Decisions API
  slug: us-patent-and-trademark-office-ptab-trials-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-ptab-trials-decisions-api-openapi.yml
- filename: us-patent-and-trademark-office-ptab-trials-documents-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office PTAB Trials Documents API
  slug: us-patent-and-trademark-office-ptab-trials-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-ptab-trials-documents-api-openapi.yml
- filename: us-patent-and-trademark-office-ptab-trials-proceedings-api-openapi.yml
  format: yaml
  label: US Patent and Trademark Office PTAB Trials Proceedings API
  slug: us-patent-and-trademark-office-ptab-trials-proceedings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/openapi/us-patent-and-trademark-office-ptab-trials-proceedings-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Us Patent And Trademark Office Authentication
name_suffix: Authentication
oauth_flows: []
overview: US Patent and Trademark Office secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: US Patent and Trademark Office
provider_slug: us-patent-and-trademark-office
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/uspto-open-data-portal-openapi.yml
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: USPTO-API-KEY
  sources:
  - openapi/uspto-tsdr-openapi.yml
  type: apiKey
slug: us-patent-and-trademark-office-authentication
source_filename: us-patent-and-trademark-office-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uspto-open-data-portal-openapi.yml, openapi/uspto-tsdr-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/uspto-open-data-portal-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: USPTO-API-KEY\n  sources:\n  - openapi/uspto-tsdr-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-patent-and-trademark-office/refs/heads/main/authentication/us-patent-and-trademark-office-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Federal Government
- Patents
- Trademarks
- Intellectual Property
- Open Data
---
