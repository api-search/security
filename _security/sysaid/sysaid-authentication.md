---
api_key_in: []
api_specs:
- filename: sysaid-actionitems-api-openapi.yml
  format: yaml
  label: SysAid ActionItems API
  slug: sysaid-actionitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-actionitems-api-openapi.yml
- filename: sysaid-activities-api-openapi.yml
  format: yaml
  label: SysAid Activities API
  slug: sysaid-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-activities-api-openapi.yml
- filename: sysaid-agents-api-openapi.yml
  format: yaml
  label: SysAid Agents API
  slug: sysaid-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-agents-api-openapi.yml
- filename: sysaid-assets-api-openapi.yml
  format: yaml
  label: SysAid Assets API
  slug: sysaid-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-assets-api-openapi.yml
- filename: sysaid-attachments-api-openapi.yml
  format: yaml
  label: SysAid Attachments API
  slug: sysaid-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-attachments-api-openapi.yml
- filename: sysaid-auth-api-openapi.yml
  format: yaml
  label: SysAid Auth API
  slug: sysaid-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-auth-api-openapi.yml
- filename: sysaid-cis-api-openapi.yml
  format: yaml
  label: SysAid CIs API
  slug: sysaid-cis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-cis-api-openapi.yml
- filename: sysaid-companies-api-openapi.yml
  format: yaml
  label: SysAid Companies API
  slug: sysaid-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-companies-api-openapi.yml
- filename: sysaid-endusers-api-openapi.yml
  format: yaml
  label: SysAid EndUsers API
  slug: sysaid-endusers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-endusers-api-openapi.yml
- filename: sysaid-groups-api-openapi.yml
  format: yaml
  label: SysAid Groups API
  slug: sysaid-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-groups-api-openapi.yml
- filename: sysaid-licensemanager-api-openapi.yml
  format: yaml
  label: SysAid LicenseManager API
  slug: sysaid-licensemanager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-licensemanager-api-openapi.yml
- filename: sysaid-relateditems-api-openapi.yml
  format: yaml
  label: SysAid RelatedItems API
  slug: sysaid-relateditems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-relateditems-api-openapi.yml
- filename: sysaid-servicerecords-api-openapi.yml
  format: yaml
  label: SysAid ServiceRecords API
  slug: sysaid-servicerecords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-servicerecords-api-openapi.yml
- filename: sysaid-templates-api-openapi.yml
  format: yaml
  label: SysAid Templates API
  slug: sysaid-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-templates-api-openapi.yml
- filename: sysaid-utilities-api-openapi.yml
  format: yaml
  label: SysAid Utilities API
  slug: sysaid-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-utilities-api-openapi.yml
- filename: sysaid-webhooks-api-openapi.yml
  format: yaml
  label: SysAid Webhooks API
  slug: sysaid-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/openapi/sysaid-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sysaid Authentication
name_suffix: Authentication
oauth_flows: []
overview: SysAid secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SysAid
provider_slug: sysaid
scheme_count: 1
schemes:
- description: 'OAuth 2.0 Client Credentials grant: exchange client_id and client_secret at /generateaccesstoken for a short-lived access token (default 24h), then pass as "Authorization: Bearer <token>".'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sysaid-openapi.yml
  type: http
slug: sysaid-authentication
source_filename: sysaid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sysaid-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth 2.0 Client Credentials grant: exchange client_id and client_secret at\n    /generateaccesstoken for a short-lived access token (default 24h), then pass as \"Authorization:\n    Bearer <token>\".'\n  sources:\n  - openapi/sysaid-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sysaid/refs/heads/main/authentication/sysaid-authentication.yml
summary_line: http · 1 scheme
tags:
- ITSM
- Help Desk
- Asset Management
- Ticketing
- Service Desk
---
