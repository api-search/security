---
api_key_in: []
api_specs:
- filename: gitbook-change-request-content-api-openapi.yml
  format: yaml
  label: GitBook Change Request Content API
  slug: gitbook-change-request-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-change-request-content-api-openapi.yml
- filename: gitbook-change-request-reviewers-api-openapi.yml
  format: yaml
  label: GitBook Change Request Reviewers API
  slug: gitbook-change-request-reviewers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-change-request-reviewers-api-openapi.yml
- filename: gitbook-change-requests-api-openapi.yml
  format: yaml
  label: GitBook Change Requests API
  slug: gitbook-change-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-change-requests-api-openapi.yml
- filename: gitbook-collections-api-openapi.yml
  format: yaml
  label: GitBook Collections API
  slug: gitbook-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-collections-api-openapi.yml
- filename: gitbook-custom-hostnames-api-openapi.yml
  format: yaml
  label: GitBook Custom Hostnames API
  slug: gitbook-custom-hostnames-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-custom-hostnames-api-openapi.yml
- filename: gitbook-docs-sites-api-openapi.yml
  format: yaml
  label: GitBook Docs Sites API
  slug: gitbook-docs-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-docs-sites-api-openapi.yml
- filename: gitbook-imports-api-openapi.yml
  format: yaml
  label: GitBook Imports API
  slug: gitbook-imports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-imports-api-openapi.yml
- filename: gitbook-integrations-api-openapi.yml
  format: yaml
  label: GitBook Integrations API
  slug: gitbook-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-integrations-api-openapi.yml
- filename: gitbook-openapi-specs-api-openapi.yml
  format: yaml
  label: GitBook OpenAPI Specs API
  slug: gitbook-openapi-specs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-openapi-specs-api-openapi.yml
- filename: gitbook-organization-members-api-openapi.yml
  format: yaml
  label: GitBook Organization Members API
  slug: gitbook-organization-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-organization-members-api-openapi.yml
- filename: gitbook-organization-teams-api-openapi.yml
  format: yaml
  label: GitBook Organization Teams API
  slug: gitbook-organization-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-organization-teams-api-openapi.yml
- filename: gitbook-organizations-api-openapi.yml
  format: yaml
  label: GitBook Organizations API
  slug: gitbook-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-organizations-api-openapi.yml
- filename: gitbook-search-api-openapi.yml
  format: yaml
  label: GitBook Search API
  slug: gitbook-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-search-api-openapi.yml
- filename: gitbook-site-spaces-api-openapi.yml
  format: yaml
  label: GitBook Site Spaces API
  slug: gitbook-site-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-site-spaces-api-openapi.yml
- filename: gitbook-space-content-api-openapi.yml
  format: yaml
  label: GitBook Space Content API
  slug: gitbook-space-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-space-content-api-openapi.yml
- filename: gitbook-space-users-api-openapi.yml
  format: yaml
  label: GitBook Space Users API
  slug: gitbook-space-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-space-users-api-openapi.yml
- filename: gitbook-spaces-api-openapi.yml
  format: yaml
  label: GitBook Spaces API
  slug: gitbook-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-spaces-api-openapi.yml
- filename: gitbook-urls-api-openapi.yml
  format: yaml
  label: GitBook URLs API
  slug: gitbook-urls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-urls-api-openapi.yml
- filename: gitbook-users-api-openapi.yml
  format: yaml
  label: GitBook Users API
  slug: gitbook-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/openapi/gitbook-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gitbook Authentication
name_suffix: Authentication
oauth_flows: []
overview: GitBook secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GitBook
provider_slug: gitbook
scheme_count: 1
schemes:
- bearerFormat: token
  description: API access token. Generate one from the Developer settings of your GitBook user account.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gitbook-gitbook-api-openapi.yml
  type: http
slug: gitbook-authentication
source_filename: gitbook-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gitbook-gitbook-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: API access token. Generate one from the Developer settings of your GitBook user\n    account.\n  sources:\n  - openapi/gitbook-gitbook-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitbook/refs/heads/main/authentication/gitbook-authentication.yml
summary_line: http · 1 scheme
tags:
- Content
- Documentation
- Experience
- Integration
- Platform
- SDK
---
