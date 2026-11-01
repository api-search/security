---
anonymous_access: false
api_key_in: []
api_specs:
- filename: quickbase-apps-api-openapi.yml
  format: yaml
  label: Quickbase Apps API
  slug: quickbase-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-apps-api-openapi.yml
- filename: quickbase-audit-api-openapi.yml
  format: yaml
  label: Quickbase Audit API
  slug: quickbase-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-audit-api-openapi.yml
- filename: quickbase-auth-api-openapi.yml
  format: yaml
  label: Quickbase Auth API
  slug: quickbase-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-auth-api-openapi.yml
- filename: quickbase-document-templates-api-openapi.yml
  format: yaml
  label: Quickbase Document Templates API
  slug: quickbase-document-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-document-templates-api-openapi.yml
- filename: quickbase-fields-api-openapi.yml
  format: yaml
  label: Quickbase Fields API
  slug: quickbase-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-fields-api-openapi.yml
- filename: quickbase-files-api-openapi.yml
  format: yaml
  label: Quickbase Files API
  slug: quickbase-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-files-api-openapi.yml
- filename: quickbase-formulas-api-openapi.yml
  format: yaml
  label: Quickbase Formulas API
  slug: quickbase-formulas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-formulas-api-openapi.yml
- filename: quickbase-groups-api-openapi.yml
  format: yaml
  label: Quickbase Groups API
  slug: quickbase-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-groups-api-openapi.yml
- filename: quickbase-platform-analytics-api-openapi.yml
  format: yaml
  label: Quickbase Platform Analytics API
  slug: quickbase-platform-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-platform-analytics-api-openapi.yml
- filename: quickbase-records-api-openapi.yml
  format: yaml
  label: Quickbase Records API
  slug: quickbase-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-records-api-openapi.yml
- filename: quickbase-reports-api-openapi.yml
  format: yaml
  label: Quickbase Reports API
  slug: quickbase-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-reports-api-openapi.yml
- filename: quickbase-solutions-api-openapi.yml
  format: yaml
  label: Quickbase Solutions API
  slug: quickbase-solutions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-solutions-api-openapi.yml
- filename: quickbase-tables-api-openapi.yml
  format: yaml
  label: Quickbase Tables API
  slug: quickbase-tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-tables-api-openapi.yml
- filename: quickbase-trustees-api-openapi.yml
  format: yaml
  label: Quickbase Trustees API
  slug: quickbase-trustees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-trustees-api-openapi.yml
- filename: quickbase-users-api-openapi.yml
  format: yaml
  label: Quickbase Users API
  slug: quickbase-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-users-api-openapi.yml
- filename: quickbase-user-token-api-openapi.yml
  format: yaml
  label: Quickbase User Token API
  slug: quickbase-user-token-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quickbase/openapi/quickbase-user-token-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Quickbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quickbase declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Quickbase
provider_slug: quickbase
scheme_count: 3
schemes:
- description: Permanent user token for authentication
  docs: https://developer.quickbase.com/auth
  in: header
  name: QB-USER-TOKEN
  type: apiKey
- description: Temporary token for client-side utilities
  docs: https://developer.quickbase.com/auth
  in: header
  name: QB-TEMP-TOKEN
  type: apiKey
- description: Can be used with Secure links on runQuery and runReport
  docs: https://developer.quickbase.com/auth
  in: header
  name: QB-ACCESS-KEY
  type: apiKey
slug: quickbase-authentication
source_filename: quickbase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: searched\nsource: https://developer.quickbase.com/auth\ndocs: https://developer.quickbase.com/auth\nschemes:\n- type: apiKey\n  name: QB-USER-TOKEN\n  in: header\n  description: Permanent user token for authentication\n  docs: https://developer.quickbase.com/auth\n- type: apiKey\n  name: QB-TEMP-TOKEN\n  in: header\n  description: Temporary token for client-side utilities\n  docs: https://developer.quickbase.com/auth\n- type: apiKey\n  name: QB-ACCESS-KEY\n  in: header\n  description: Can be used with Secure links on runQuery and runReport\n  docs: https://developer.quickbase.com/auth\nnote: Quickbase uses API key authentication via custom headers. User tokens can be permanent or temporary. SSO tokens can be exchanged for Quickbase tokens via the Exchange an SSO token endpoint."
source_yaml_url: https://artifacts.apis.io/quickbase/authentication/quickbase-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Low-Code
- No-Code
- Application Development
- Project Management
- Workflow Automation
- Databases
---
