---
api_key_in: []
api_specs:
- filename: affinda-documents-api-openapi.yml
  format: yaml
  label: Affinda Documents API
  slug: affinda-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-documents-api-openapi.yml
- filename: affinda-document-types-api-openapi.yml
  format: yaml
  label: Affinda Document Types API
  slug: affinda-document-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-document-types-api-openapi.yml
- filename: affinda-extractors-api-openapi.yml
  format: yaml
  label: Affinda Extractors API
  slug: affinda-extractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-extractors-api-openapi.yml
- filename: affinda-document-splitters-api-openapi.yml
  format: yaml
  label: Affinda Document Splitters API
  slug: affinda-document-splitters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-document-splitters-api-openapi.yml
- filename: affinda-workspaces-api-openapi.yml
  format: yaml
  label: Affinda Workspaces API
  slug: affinda-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-workspaces-api-openapi.yml
- filename: affinda-organizations-api-openapi.yml
  format: yaml
  label: Affinda Organizations API
  slug: affinda-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-organizations-api-openapi.yml
- filename: affinda-invitations-api-openapi.yml
  format: yaml
  label: Affinda Invitations API
  slug: affinda-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-invitations-api-openapi.yml
- filename: affinda-data-sources-api-openapi.yml
  format: yaml
  label: Affinda Data Sources API
  slug: affinda-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-data-sources-api-openapi.yml
- filename: affinda-annotations-api-openapi.yml
  format: yaml
  label: Affinda Annotations API
  slug: affinda-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-annotations-api-openapi.yml
- filename: affinda-validation-results-api-openapi.yml
  format: yaml
  label: Affinda Validation Results API
  slug: affinda-validation-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-validation-results-api-openapi.yml
- filename: affinda-tags-api-openapi.yml
  format: yaml
  label: Affinda Tags API
  slug: affinda-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-tags-api-openapi.yml
- filename: affinda-usage-api-openapi.yml
  format: yaml
  label: Affinda Usage API
  slug: affinda-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-usage-api-openapi.yml
- filename: affinda-webhooks-api-openapi.yml
  format: yaml
  label: Affinda Webhooks API
  slug: affinda-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-webhooks-api-openapi.yml
- filename: affinda-search-match-api-openapi.yml
  format: yaml
  label: Affinda Search and Match API
  slug: affinda-search-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/openapi/affinda-search-match-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Affinda Authentication
name_suffix: Authentication
oauth_flows: []
overview: Affinda secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Affinda
provider_slug: affinda
scheme_count: 1
schemes:
- description: 'Basic authentication using an API key, e.g. `{Authorization: Bearer aff_0bb4fbdf97b7e4111ff6c0015471094155f91}`.

    You can find your API key within the Settings page of the [Affinda web app](https://app.affinda.com/). You can obtain an API key by [signing up for a free trial](https://app.affinda.com/auth/register).'
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/affinda-annotations-api-openapi.yml
  - openapi/affinda-data-sources-api-openapi.yml
  - openapi/affinda-document-splitters-api-openapi.yml
  - openapi/affinda-document-types-api-openapi.yml
  - openapi/affinda-documents-api-openapi.yml
  - openapi/affinda-extractors-api-openapi.yml
  - openapi/affinda-invitations-api-openapi.yml
  - openapi/affinda-organizations-api-openapi.yml
  - openapi/affinda-search-match-api-openapi.yml
  - openapi/affinda-tags-api-openapi.yml
  - openapi/affinda-usage-api-openapi.yml
  - openapi/affinda-v3-openapi.yml
  - openapi/affinda-validation-results-api-openapi.yml
  - openapi/affinda-webhooks-api-openapi.yml
  - openapi/affinda-workspaces-api-openapi.yml
  type: http
slug: affinda-authentication
source_filename: affinda-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/affinda-annotations-api-openapi.yml, openapi/affinda-data-sources-api-openapi.yml,\n  openapi/affinda-document-splitters-api-openapi.yml, openapi/affinda-document-types-api-openapi.yml,\n  openapi/affinda-documents-api-openapi.yml, openapi/affinda-extractors-api-openapi.yml, openapi/affinda-invitations-api-openapi.yml,\n  openapi/affinda-organizations-api-openapi.yml, openapi/affinda-search-match-api-openapi.yml,\n  openapi/affinda-tags-api-openapi.yml, openapi/affinda-usage-api-openapi.yml, openapi/affinda-v3-openapi.yml\n  ...\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Basic authentication using an API key, e.g. `{Authorization: Bearer aff_0bb4fbdf97b7e4111ff6c0015471094155f91}`.\n    You can find your API key within the Settings page of the [Affinda web app](https://app.affinda.com/). You can obtain an API key by [signing up for a free trial](https://app.affinda.com/auth/register).\n\
  \  sources:\n  - openapi/affinda-annotations-api-openapi.yml\n  - openapi/affinda-data-sources-api-openapi.yml\n  - openapi/affinda-document-splitters-api-openapi.yml\n  - openapi/affinda-document-types-api-openapi.yml\n  - openapi/affinda-documents-api-openapi.yml\n  - openapi/affinda-extractors-api-openapi.yml\n  - openapi/affinda-invitations-api-openapi.yml\n  - openapi/affinda-organizations-api-openapi.yml\n  - openapi/affinda-search-match-api-openapi.yml\n  - openapi/affinda-tags-api-openapi.yml\n  - openapi/affinda-usage-api-openapi.yml\n  - openapi/affinda-v3-openapi.yml\n  - openapi/affinda-validation-results-api-openapi.yml\n  - openapi/affinda-webhooks-api-openapi.yml\n  - openapi/affinda-workspaces-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affinda/refs/heads/main/authentication/affinda-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- Document Processing
- Intelligent Document Processing
- IDP
- OCR
- Resume Parsing
- Invoice Parsing
- Receipt Parsing
- Document Extraction
- Document Classification
- Document Splitting
- Recruitment
- Banking
- Insurance
- Logistics
- Healthcare
- Government
---
