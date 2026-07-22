---
api_key_in:
- header
auth_types:
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Onehouse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Onehouse secures its APIs with http-bearer across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Onehouse
provider_slug: onehouse
scheme_count: 1
schemes:
- description: Service Principals are created in Onehouse project settings (Identity) to generate access tokens that are used as bearer credentials to securely access Onehouse via the control-plane REST API (SQL Command API + Status API). The Onehouse CLI stores these credentials via `oh-configure`.
  name: ServicePrincipalToken
  scheme: bearer
  sources:
  - docs.onehouse.ai/product/project-settings/identity/service-principals
  type: http
slug: onehouse-authentication
source_filename: onehouse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.onehouse.ai/product/project-settings/identity/service-principals\ndocs: https://docs.onehouse.ai/api/overview\nsummary:\n  types: [http-bearer]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: ServicePrincipalToken\n    type: http\n    scheme: bearer\n    description: >-\n      Service Principals are created in Onehouse project settings (Identity) to\n      generate access tokens that are used as bearer credentials to securely\n      access Onehouse via the control-plane REST API (SQL Command API + Status\n      API). The Onehouse CLI stores these credentials via `oh-configure`.\n    sources: [docs.onehouse.ai/product/project-settings/identity/service-principals]\nnotes:\n  - Data-plane (LakeBase / Lakegres PostgreSQL) uses standard username/password\n    plus browser-based and federated authentication flows handled by the SDK.\n  - No OpenAPI security scheme could be harvested; the control-plane\
  \ API docs are\n    gated (request-docs-access), so this profile is derived from the public docs\n    overview and service-principals reference.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onehouse/refs/heads/main/authentication/onehouse-authentication.yml
summary_line: http-bearer · 1 scheme
tags:
- Company
- Developer Tools
- Data Lakehouse
- Data Engineering
- ETL
- Apache Hudi
- Analytics
- Data Infrastructure
---
