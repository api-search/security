---
api_key_in:
- cookie
api_specs:
- filename: utrecht-admin-api-openapi.yml
  format: yaml
  label: Utrecht University admin API
  slug: utrecht-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-admin-api-openapi.yml
- filename: utrecht-browse-api-openapi.yml
  format: yaml
  label: Utrecht University browse API
  slug: utrecht-browse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-browse-api-openapi.yml
- filename: utrecht-data-access-token-api-openapi.yml
  format: yaml
  label: Utrecht University data_access_token API
  slug: utrecht-data-access-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-data-access-token-api-openapi.yml
- filename: utrecht-datarequest-api-openapi.yml
  format: yaml
  label: Utrecht University datarequest API
  slug: utrecht-datarequest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-datarequest-api-openapi.yml
- filename: utrecht-folder-api-openapi.yml
  format: yaml
  label: Utrecht University folder API
  slug: utrecht-folder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-folder-api-openapi.yml
- filename: utrecht-groups-api-openapi.yml
  format: yaml
  label: Utrecht University groups API
  slug: utrecht-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-groups-api-openapi.yml
- filename: utrecht-meta-api-openapi.yml
  format: yaml
  label: Utrecht University meta API
  slug: utrecht-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-meta-api-openapi.yml
- filename: utrecht-meta-form-api-openapi.yml
  format: yaml
  label: Utrecht University meta_form API
  slug: utrecht-meta-form-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-meta-form-api-openapi.yml
- filename: utrecht-notifications-api-openapi.yml
  format: yaml
  label: Utrecht University notifications API
  slug: utrecht-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-notifications-api-openapi.yml
- filename: utrecht-provenance-api-openapi.yml
  format: yaml
  label: Utrecht University provenance API
  slug: utrecht-provenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-provenance-api-openapi.yml
- filename: utrecht-publication-troubleshoot-api-openapi.yml
  format: yaml
  label: Utrecht University publication_troubleshoot API
  slug: utrecht-publication-troubleshoot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-publication-troubleshoot-api-openapi.yml
- filename: utrecht-research-api-openapi.yml
  format: yaml
  label: Utrecht University research API
  slug: utrecht-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-research-api-openapi.yml
- filename: utrecht-revisions-api-openapi.yml
  format: yaml
  label: Utrecht University revisions API
  slug: utrecht-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-revisions-api-openapi.yml
- filename: utrecht-schema-api-openapi.yml
  format: yaml
  label: Utrecht University schema API
  slug: utrecht-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-schema-api-openapi.yml
- filename: utrecht-schema-transformation-api-openapi.yml
  format: yaml
  label: Utrecht University schema_transformation API
  slug: utrecht-schema-transformation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-schema-transformation-api-openapi.yml
- filename: utrecht-settings-api-openapi.yml
  format: yaml
  label: Utrecht University settings API
  slug: utrecht-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-settings-api-openapi.yml
- filename: utrecht-stats-api-openapi.yml
  format: yaml
  label: Utrecht University stats API
  slug: utrecht-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-stats-api-openapi.yml
- filename: utrecht-vault-api-openapi.yml
  format: yaml
  label: Utrecht University vault API
  slug: utrecht-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-vault-api-openapi.yml
- filename: utrecht-vault-archive-api-openapi.yml
  format: yaml
  label: Utrecht University vault_archive API
  slug: utrecht-vault-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-vault-archive-api-openapi.yml
- filename: utrecht-vault-deaccession-api-openapi.yml
  format: yaml
  label: Utrecht University vault_deaccession API
  slug: utrecht-vault-deaccession-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-vault-deaccession-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Utrecht Authentication
name_suffix: Authentication
oauth_flows: []
overview: Utrecht University secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Utrecht University
provider_slug: utrecht
scheme_count: 2
schemes:
- in: cookie
  name: cookieAuth
  parameter: yoda_session
  sources:
  - openapi/utrecht-yoda-core.yaml
  - openapi/utrecht-yoda-datarequest.yaml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/utrecht-yoda-core.yaml
  - openapi/utrecht-yoda-datarequest.yaml
  type: http
slug: utrecht-authentication
source_filename: utrecht-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/utrecht-yoda-core.yaml, openapi/utrecht-yoda-datarequest.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: yoda_session\n  sources:\n  - openapi/utrecht-yoda-core.yaml\n  - openapi/utrecht-yoda-datarequest.yaml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/utrecht-yoda-core.yaml\n  - openapi/utrecht-yoda-datarequest.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/authentication/utrecht-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Education
- Higher Education
- University
- Netherlands
- Research Data
- Open Access
- Library
- Open-Source
---
