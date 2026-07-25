---
api_key_in: []
api_specs:
- filename: lumos-accesspolicies-api-openapi.yml
  format: yaml
  label: Lumos AccessPolicies API
  slug: lumos-accesspolicies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accesspolicies-api-openapi.yml
- filename: lumos-accessrequests-api-openapi.yml
  format: yaml
  label: Lumos AccessRequests API
  slug: lumos-accessrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accessrequests-api-openapi.yml
- filename: lumos-accessreviews-api-openapi.yml
  format: yaml
  label: Lumos AccessReviews API
  slug: lumos-accessreviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accessreviews-api-openapi.yml
- filename: lumos-accounts-api-openapi.yml
  format: yaml
  label: Lumos Accounts API
  slug: lumos-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-accounts-api-openapi.yml
- filename: lumos-activity-api-openapi.yml
  format: yaml
  label: Lumos Activity API
  slug: lumos-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-activity-api-openapi.yml
- filename: lumos-apps-api-openapi.yml
  format: yaml
  label: Lumos Apps API
  slug: lumos-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-apps-api-openapi.yml
- filename: lumos-appstore-api-openapi.yml
  format: yaml
  label: Lumos AppStore API
  slug: lumos-appstore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-appstore-api-openapi.yml
- filename: lumos-groups-api-openapi.yml
  format: yaml
  label: Lumos Groups API
  slug: lumos-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-groups-api-openapi.yml
- filename: lumos-preapprovalrules-api-openapi.yml
  format: yaml
  label: Lumos PreApprovalRules API
  slug: lumos-preapprovalrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-preapprovalrules-api-openapi.yml
- filename: lumos-tasks-api-openapi.yml
  format: yaml
  label: Lumos Tasks API
  slug: lumos-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-tasks-api-openapi.yml
- filename: lumos-users-api-openapi.yml
  format: yaml
  label: Lumos Users API
  slug: lumos-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-users-api-openapi.yml
- filename: lumos-utility-api-openapi.yml
  format: yaml
  label: Lumos Utility API
  slug: lumos-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-utility-api-openapi.yml
- filename: lumos-vendors-api-openapi.yml
  format: yaml
  label: Lumos Vendors API
  slug: lumos-vendors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-vendors-api-openapi.yml
- filename: lumos-webhooks-api-openapi.yml
  format: yaml
  label: Lumos Webhooks API
  slug: lumos-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/openapi/lumos-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lumos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lumos secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lumos
provider_slug: lumos
scheme_count: 1
schemes:
- bearerFormat: Lumos API key (lsk_ prefix)
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/lumos-openapi.yml
  type: http
slug: lumos-authentication
source_filename: lumos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lumos-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Lumos API key (lsk_ prefix)\n  sources:\n  - openapi/lumos-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumos/refs/heads/main/authentication/lumos-authentication.yml
summary_line: http · 1 scheme
tags:
- Access Management
- Access Reviews
- Deprovisioning
- Identity Governance
- Identity Platform
- Least Privilege
- Provisioning
- SaaS Management
- Shadow IT
---
