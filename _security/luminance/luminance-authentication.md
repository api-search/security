---
api_key_in: []
api_specs:
- filename: luminance-accounts-api-openapi.yml
  format: yaml
  label: Luminance Accounts API
  slug: luminance-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-accounts-api-openapi.yml
- filename: luminance-annotation-source-relations-api-openapi.yml
  format: yaml
  label: Luminance Annotation Source Relations API
  slug: luminance-annotation-source-relations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-annotation-source-relations-api-openapi.yml
- filename: luminance-annotation-sources-api-openapi.yml
  format: yaml
  label: Luminance Annotation Sources API
  slug: luminance-annotation-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-annotation-sources-api-openapi.yml
- filename: luminance-annotation-types-api-openapi.yml
  format: yaml
  label: Luminance Annotation Types API
  slug: luminance-annotation-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-annotation-types-api-openapi.yml
- filename: luminance-annotations-api-openapi.yml
  format: yaml
  label: Luminance Annotations API
  slug: luminance-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-annotations-api-openapi.yml
- filename: luminance-contract-creation-api-openapi.yml
  format: yaml
  label: Luminance Contract Creation API
  slug: luminance-contract-creation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-contract-creation-api-openapi.yml
- filename: luminance-document-templates-api-openapi.yml
  format: yaml
  label: Luminance Document Templates API
  slug: luminance-document-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-document-templates-api-openapi.yml
- filename: luminance-documents-api-openapi.yml
  format: yaml
  label: Luminance Documents API
  slug: luminance-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-documents-api-openapi.yml
- filename: luminance-folders-api-openapi.yml
  format: yaml
  label: Luminance Folders API
  slug: luminance-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-folders-api-openapi.yml
- filename: luminance-matter-versions-api-openapi.yml
  format: yaml
  label: Luminance Matter Versions API
  slug: luminance-matter-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-matter-versions-api-openapi.yml
- filename: luminance-matters-api-openapi.yml
  format: yaml
  label: Luminance Matters API
  slug: luminance-matters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-matters-api-openapi.yml
- filename: luminance-project-users-api-openapi.yml
  format: yaml
  label: Luminance Project Users API
  slug: luminance-project-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-project-users-api-openapi.yml
- filename: luminance-projects-api-openapi.yml
  format: yaml
  label: Luminance Projects API
  slug: luminance-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-projects-api-openapi.yml
- filename: luminance-reviews-api-openapi.yml
  format: yaml
  label: Luminance Reviews API
  slug: luminance-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-reviews-api-openapi.yml
- filename: luminance-root-api-openapi.yml
  format: yaml
  label: Luminance Root API
  slug: luminance-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-root-api-openapi.yml
- filename: luminance-search-api-openapi.yml
  format: yaml
  label: Luminance Search API
  slug: luminance-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-search-api-openapi.yml
- filename: luminance-system-api-openapi.yml
  format: yaml
  label: Luminance System API
  slug: luminance-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-system-api-openapi.yml
- filename: luminance-tasks-api-openapi.yml
  format: yaml
  label: Luminance Tasks API
  slug: luminance-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-tasks-api-openapi.yml
- filename: luminance-traffic-light-analysis-api-openapi.yml
  format: yaml
  label: Luminance Traffic Light Analysis API
  slug: luminance-traffic-light-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-traffic-light-analysis-api-openapi.yml
- filename: luminance-users-api-openapi.yml
  format: yaml
  label: Luminance Users API
  slug: luminance-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-users-api-openapi.yml
- filename: luminance-workflows-api-openapi.yml
  format: yaml
  label: Luminance Workflows API
  slug: luminance-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/openapi/luminance-workflows-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Luminance Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Luminance secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Luminance
provider_slug: luminance
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://moniker.app.luminance.com/auth/oauth2/token
  name: OAuth2
  sources:
  - openapi/luminance-api-v1-3-openapi-original.yml
  - openapi/luminance-api-v1-4-openapi-original.yml
  type: oauth2
- bearerFormat: JWT
  description: Access token from the OAuth2 client credentials flow. See the Authentication section above for how to obtain a token (curl to your instance token endpoint); then paste the access_token here.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/luminance-public-api-v2-openapi-original.yml
  type: http
slug: luminance-authentication
source_filename: luminance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: derived\nsource: openapi/luminance-api-v1-3-openapi-original.yml, openapi/luminance-api-v1-4-openapi-original.yml,\n  openapi/luminance-public-api-v2-openapi-original.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://moniker.app.luminance.com/auth/oauth2/token\n    scopes: 0\n  sources:\n  - openapi/luminance-api-v1-3-openapi-original.yml\n  - openapi/luminance-api-v1-4-openapi-original.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Access token from the OAuth2 client credentials flow. See the Authentication\n    section above for how to obtain a token (curl to your instance token endpoint); then paste\n    the access_token here.\n  sources:\n  - openapi/luminance-public-api-v2-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luminance/refs/heads/main/authentication/luminance-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Legal
- Artificial Intelligence
- Contracts
- Contract Lifecycle Management
- Document Intelligence
- Compliance
- Legal Technology
- Enterprise Software
- Automation
---
