---
api_key_in: []
api_specs:
- filename: seven-bridges-action-api-openapi.yml
  format: yaml
  label: Seven Bridges Action API
  slug: seven-bridges-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-action-api-openapi.yml
- filename: seven-bridges-api-settings-api-openapi.yml
  format: yaml
  label: Seven Bridges API Settings API
  slug: seven-bridges-api-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-api-settings-api-openapi.yml
- filename: seven-bridges-apps-api-openapi.yml
  format: yaml
  label: Seven Bridges Apps API
  slug: seven-bridges-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-apps-api-openapi.yml
- filename: seven-bridges-billing-api-openapi.yml
  format: yaml
  label: Seven Bridges Billing API
  slug: seven-bridges-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-billing-api-openapi.yml
- filename: seven-bridges-bulk-api-openapi.yml
  format: yaml
  label: Seven Bridges Bulk API
  slug: seven-bridges-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-bulk-api-openapi.yml
- filename: seven-bridges-files-api-openapi.yml
  format: yaml
  label: Seven Bridges Files API
  slug: seven-bridges-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-files-api-openapi.yml
- filename: seven-bridges-https-api-openapi.yml
  format: yaml
  label: 'Seven Bridges Https: API'
  slug: seven-bridges-https-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-https-api-openapi.yml
- filename: seven-bridges-projects-api-openapi.yml
  format: yaml
  label: Seven Bridges Projects API
  slug: seven-bridges-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-projects-api-openapi.yml
- filename: seven-bridges-rate-limit-api-openapi.yml
  format: yaml
  label: Seven Bridges Rate Limit API
  slug: seven-bridges-rate-limit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-rate-limit-api-openapi.yml
- filename: seven-bridges-search-api-openapi.yml
  format: yaml
  label: Seven Bridges Search API
  slug: seven-bridges-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-search-api-openapi.yml
- filename: seven-bridges-seven-bridges-platform-api-openapi.yml
  format: yaml
  label: Seven Bridges Seven Bridges Platform API
  slug: seven-bridges-seven-bridges-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-seven-bridges-platform-api-openapi.yml
- filename: seven-bridges-storage-api-openapi.yml
  format: yaml
  label: Seven Bridges Storage API
  slug: seven-bridges-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-storage-api-openapi.yml
- filename: seven-bridges-tasks-api-openapi.yml
  format: yaml
  label: Seven Bridges Tasks API
  slug: seven-bridges-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-tasks-api-openapi.yml
- filename: seven-bridges-upload-api-openapi.yml
  format: yaml
  label: Seven Bridges Upload API
  slug: seven-bridges-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-upload-api-openapi.yml
- filename: seven-bridges-user-api-openapi.yml
  format: yaml
  label: Seven Bridges User API
  slug: seven-bridges-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-user-api-openapi.yml
- filename: seven-bridges-users-api-openapi.yml
  format: yaml
  label: Seven Bridges Users API
  slug: seven-bridges-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/openapi/seven-bridges-users-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Seven Bridges Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seven Bridges declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Seven Bridges
provider_slug: seven-bridges
scheme_count: 1
schemes:
- description: Per-user authentication token issued from the Platform developer dashboard. Sent as an HTTP request header on every call. The only documented exemption is GET / (list all API paths), which is anonymous.
  in: header
  name: X-SBG-Auth-Token
  parameter: X-SBG-Auth-Token
  rotation: Tokens are regenerated from the developer dashboard; the docs do not publish an expiry, a scope model, or a programmatic token-issuance endpoint.
  type: apiKey
  where_to_get: https://igor.sbgenomics.com/developer#token
slug: seven-bridges-authentication
source_filename: seven-bridges-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://docs.sevenbridges.com/docs/the-api\ndocs: https://docs.sevenbridges.com/docs/get-your-authentication-token\nnote: >-\n  The ReadMe-exported OpenAPI carries an empty components.securitySchemes block, so the auth model was read\n  from the provider's own API overview and token documentation rather than derived from the spec. Every\n  operation in the spec except GET / does carry an X-SBG-Auth-Token header parameter (82 of 91 operations),\n  which corroborates the documented model.\nmodel: api-key\nschemes:\n- name: X-SBG-Auth-Token\n  type: apiKey\n  in: header\n  parameter: X-SBG-Auth-Token\n  description: >-\n    Per-user authentication token issued from the Platform developer dashboard. Sent as an HTTP request\n    header on every call. The only documented exemption is GET / (list all API paths), which is anonymous.\n  where_to_get: https://igor.sbgenomics.com/developer#token\n  rotation: >-\n    Tokens are regenerated\
  \ from the developer dashboard; the docs do not publish an expiry, a scope model,\n    or a programmatic token-issuance endpoint.\noauth2: false\nopenid_connect: false\nmutual_tls: false\nscopes: false\nscopes_note: >-\n  Authorization is not scope-based. Access is governed by per-project and per-volume member permissions\n  (read, write, copy, execute, admin) managed through the /projects/{owner}/{project}/members and\n  /storage/volumes/{owner}/{name}/members operations, and the API returns 403 with a numeric platform\n  error code when a caller lacks the required permission.\nanonymous_endpoints:\n- operationId: list-all-api-paths\n  path: /\n  method: GET\n  note: Returns the hypermedia index of API resource URLs without a token; verified live 2026-08-27 (HTTP 200).\ntoken_storage: >-\n  The Seven Bridges client libraries and the `sb` CLI read credentials from a shared configuration file;\n  see https://docs.sevenbridges.com/docs/store-credentials-to-access-seven-bridges-client-applications-and-libraries\n\
  regional_endpoints:\n- region: AWS US\n  base: https://api.sbgenomics.com/v2\n- region: AWS EU\n  base: https://eu-api.sbgenomics.com/v2\n- region: Cancer Genomics Cloud\n  base: https://cgc-api.sbgenomics.com/v2\n  token_source: https://cgc.sbgenomics.com/developer\n- region: CAVATICA\n  base: https://cavatica-api.sbgenomics.com/v2\n  token_source: https://cavatica.sbgenomics.com/developer\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seven-bridges/refs/heads/main/authentication/seven-bridges-authentication.yml
summary_line: 1 scheme
tags:
- Genomics
- Bioinformatics
- Life Sciences
- Healthcare
- Cloud Computing
- Data Analysis
- Workflow Automation
- Research
- Precision Medicine
- Common Workflow Language
- File Storage
- Company
---
