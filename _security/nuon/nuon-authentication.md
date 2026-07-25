---
api_key_in:
- header
api_specs:
- filename: nuon-accounts-api-openapi.yml
  format: yaml
  label: Nuon accounts API
  slug: nuon-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-accounts-api-openapi.yml
- filename: nuon-actions-api-openapi.yml
  format: yaml
  label: Nuon actions API
  slug: nuon-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-actions-api-openapi.yml
- filename: nuon-actions-runner-api-openapi.yml
  format: yaml
  label: Nuon actions/runner API
  slug: nuon-actions-runner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-actions-runner-api-openapi.yml
- filename: nuon-apps-api-openapi.yml
  format: yaml
  label: Nuon apps API
  slug: nuon-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-apps-api-openapi.yml
- filename: nuon-auth-api-openapi.yml
  format: yaml
  label: Nuon auth API
  slug: nuon-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-auth-api-openapi.yml
- filename: nuon-components-api-openapi.yml
  format: yaml
  label: Nuon components API
  slug: nuon-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-components-api-openapi.yml
- filename: nuon-general-api-openapi.yml
  format: yaml
  label: Nuon general API
  slug: nuon-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-general-api-openapi.yml
- filename: nuon-installs-api-openapi.yml
  format: yaml
  label: Nuon installs API
  slug: nuon-installs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-installs-api-openapi.yml
- filename: nuon-notebooks-api-openapi.yml
  format: yaml
  label: Nuon notebooks API
  slug: nuon-notebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-notebooks-api-openapi.yml
- filename: nuon-onboarding-api-openapi.yml
  format: yaml
  label: Nuon onboarding API
  slug: nuon-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-onboarding-api-openapi.yml
- filename: nuon-orgs-api-openapi.yml
  format: yaml
  label: Nuon orgs API
  slug: nuon-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-orgs-api-openapi.yml
- filename: nuon-policy-reports-api-openapi.yml
  format: yaml
  label: Nuon policy-reports API
  slug: nuon-policy-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-policy-reports-api-openapi.yml
- filename: nuon-queues-api-openapi.yml
  format: yaml
  label: Nuon queues API
  slug: nuon-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-queues-api-openapi.yml
- filename: nuon-runbooks-api-openapi.yml
  format: yaml
  label: Nuon runbooks API
  slug: nuon-runbooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-runbooks-api-openapi.yml
- filename: nuon-runners-api-openapi.yml
  format: yaml
  label: Nuon runners API
  slug: nuon-runners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-runners-api-openapi.yml
- filename: nuon-runners-runner-api-openapi.yml
  format: yaml
  label: Nuon runners/runner API
  slug: nuon-runners-runner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-runners-runner-api-openapi.yml
- filename: nuon-slack-api-openapi.yml
  format: yaml
  label: Nuon slack API
  slug: nuon-slack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-slack-api-openapi.yml
- filename: nuon-vcs-api-openapi.yml
  format: yaml
  label: Nuon vcs API
  slug: nuon-vcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-vcs-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nuon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nuon secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nuon
provider_slug: nuon
scheme_count: 2
schemes:
- description: Type "Bearer" followed by a space and token.
  in: header
  name: APIKey
  parameter: Authorization
  sources:
  - openapi/nuon-oapi-v2-openapi.json
  - openapi/nuon-oapi-v3-openapi.json
  type: apiKey
- description: Nuon org ID
  in: header
  name: OrgID
  parameter: X-Nuon-Org-ID
  sources:
  - openapi/nuon-oapi-v2-openapi.json
  - openapi/nuon-oapi-v3-openapi.json
  type: apiKey
slug: nuon-authentication
source_filename: nuon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/nuon-oapi-v2-openapi.json, openapi/nuon-oapi-v3-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Type \"Bearer\" followed by a space and token.\n  sources:\n  - openapi/nuon-oapi-v2-openapi.json\n  - openapi/nuon-oapi-v3-openapi.json\n- name: OrgID\n  type: apiKey\n  in: header\n  parameter: X-Nuon-Org-ID\n  description: Nuon org ID\n  sources:\n  - openapi/nuon-oapi-v2-openapi.json\n  - openapi/nuon-oapi-v3-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/authentication/nuon-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- BYOC
- Deployment
- Continuous Delivery
- DevOps
- Infrastructure
- Cloud
- Multi-Cloud
- Kubernetes
- Terraform
- Platform Engineering
---
