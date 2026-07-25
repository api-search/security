---
api_key_in: []
api_specs:
- filename: sedna-authentication-api-openapi.yml
  format: yaml
  label: SEDNA Authentication API
  slug: sedna-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-authentication-api-openapi.yml
- filename: sedna-category-tag-api-api-openapi.yml
  format: yaml
  label: SEDNA Category Tag API API
  slug: sedna-category-tag-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-category-tag-api-api-openapi.yml
- filename: sedna-comment-api-api-openapi.yml
  format: yaml
  label: SEDNA Comment API API
  slug: sedna-comment-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-comment-api-api-openapi.yml
- filename: sedna-company-api-api-openapi.yml
  format: yaml
  label: SEDNA Company API API
  slug: sedna-company-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-company-api-api-openapi.yml
- filename: sedna-contact-api-api-openapi.yml
  format: yaml
  label: SEDNA Contact API API
  slug: sedna-contact-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-contact-api-api-openapi.yml
- filename: sedna-document-api-api-openapi.yml
  format: yaml
  label: SEDNA Document API API
  slug: sedna-document-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-document-api-api-openapi.yml
- filename: sedna-download-api-api-openapi.yml
  format: yaml
  label: SEDNA Download API API
  slug: sedna-download-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-download-api-api-openapi.yml
- filename: sedna-event-api-api-openapi.yml
  format: yaml
  label: SEDNA Event API API
  slug: sedna-event-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-event-api-api-openapi.yml
- filename: sedna-job-reference-api-api-openapi.yml
  format: yaml
  label: SEDNA Job Reference API API
  slug: sedna-job-reference-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-job-reference-api-api-openapi.yml
- filename: sedna-keyword-api-api-openapi.yml
  format: yaml
  label: SEDNA Keyword API API
  slug: sedna-keyword-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-keyword-api-api-openapi.yml
- filename: sedna-message-api-api-openapi.yml
  format: yaml
  label: SEDNA Message API API
  slug: sedna-message-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-message-api-api-openapi.yml
- filename: sedna-saved-search-api-api-openapi.yml
  format: yaml
  label: SEDNA Saved Search API API
  slug: sedna-saved-search-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-saved-search-api-api-openapi.yml
- filename: sedna-team-api-api-openapi.yml
  format: yaml
  label: SEDNA Team API API
  slug: sedna-team-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-team-api-api-openapi.yml
- filename: sedna-template-api-api-openapi.yml
  format: yaml
  label: SEDNA Template API API
  slug: sedna-template-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-template-api-api-openapi.yml
- filename: sedna-user-api-api-openapi.yml
  format: yaml
  label: SEDNA User API API
  slug: sedna-user-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-user-api-api-openapi.yml
- filename: sedna-vessel-api-api-openapi.yml
  format: yaml
  label: SEDNA Vessel API API
  slug: sedna-vessel-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-vessel-api-api-openapi.yml
- filename: sedna-workflow-api-api-openapi.yml
  format: yaml
  label: SEDNA Workflow API API
  slug: sedna-workflow-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/openapi/sedna-workflow-api-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sedna Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SEDNA secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SEDNA
provider_slug: sedna
scheme_count: 2
schemes:
- description: The basic auth scheme only requires the API-Specific username/password to be set.
  name: Basic
  scheme: basic
  sources:
  - openapi/sedna-openapi.json
  type: http
- description: This API prefers OAuth 2 with client credentials flow. You can create your credentials in the <a href='https://{tenant}.sednanetwork.com/platform/settings/api-credential-management'>Api Credential Management page</a>.
  flows:
  - flow: clientCredentials
    scopes: 53
    tokenUrl: https://{tenant}.sednanetwork.com/platform/oauth/token
  name: OAuth
  sources:
  - openapi/sedna-openapi.json
  type: oauth2
slug: sedna-authentication
source_filename: sedna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/sedna-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  description: The basic auth scheme only requires the API-Specific username/password to be\n    set.\n  sources:\n  - openapi/sedna-openapi.json\n- name: OAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.sednanetwork.com/platform/oauth/token\n    scopes: 53\n  description: This API prefers OAuth 2 with client credentials flow. You can create your credentials\n    in the <a href='https://{tenant}.sednanetwork.com/platform/settings/api-credential-management'>Api\n    Credential Management page</a>.\n  sources:\n  - openapi/sedna-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sedna/refs/heads/main/authentication/sedna-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Shipping
- Maritime
- Email
- Communications
- Workflow
- Commodity Trading
- Logistics
- Messaging
---
