---
api_key_in: []
api_specs:
- filename: sysdig-activity-audit-api-openapi.yml
  format: yaml
  label: Sysdig Activity Audit API
  slug: sysdig-activity-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-activity-audit-api-openapi.yml
- filename: sysdig-alerts-api-openapi.yml
  format: yaml
  label: Sysdig Alerts API
  slug: sysdig-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-alerts-api-openapi.yml
- filename: sysdig-compliance-api-openapi.yml
  format: yaml
  label: Sysdig Compliance API
  slug: sysdig-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-compliance-api-openapi.yml
- filename: sysdig-dashboards-api-openapi.yml
  format: yaml
  label: Sysdig Dashboards API
  slug: sysdig-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-dashboards-api-openapi.yml
- filename: sysdig-events-api-openapi.yml
  format: yaml
  label: Sysdig Events API
  slug: sysdig-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-events-api-openapi.yml
- filename: sysdig-image-scanning-api-openapi.yml
  format: yaml
  label: Sysdig Image Scanning API
  slug: sysdig-image-scanning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-image-scanning-api-openapi.yml
- filename: sysdig-metrics-api-openapi.yml
  format: yaml
  label: Sysdig Metrics API
  slug: sysdig-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-metrics-api-openapi.yml
- filename: sysdig-notification-channels-api-openapi.yml
  format: yaml
  label: Sysdig Notification Channels API
  slug: sysdig-notification-channels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-notification-channels-api-openapi.yml
- filename: sysdig-policies-api-openapi.yml
  format: yaml
  label: Sysdig Policies API
  slug: sysdig-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-policies-api-openapi.yml
- filename: sysdig-rules-api-openapi.yml
  format: yaml
  label: Sysdig Rules API
  slug: sysdig-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-rules-api-openapi.yml
- filename: sysdig-sbom-api-openapi.yml
  format: yaml
  label: Sysdig SBOM API
  slug: sysdig-sbom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-sbom-api-openapi.yml
- filename: sysdig-teams-api-openapi.yml
  format: yaml
  label: Sysdig Teams API
  slug: sysdig-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-teams-api-openapi.yml
- filename: sysdig-vulnerabilities-api-openapi.yml
  format: yaml
  label: Sysdig Vulnerabilities API
  slug: sysdig-vulnerabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-vulnerabilities-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sysdig Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sysdig secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sysdig
provider_slug: sysdig
scheme_count: 1
schemes:
- description: Authenticate using a Sysdig API Token, Team-Based Service Account, or Global Service Account token as a Bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sysdig-monitor-openapi.yml
  - openapi/sysdig-secure-openapi.yml
  type: http
slug: sysdig-authentication
source_filename: sysdig-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sysdig-monitor-openapi.yml, openapi/sysdig-secure-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Authenticate using a Sysdig API Token, Team-Based Service Account, or Global\n    Service Account token as a Bearer token.\n  sources:\n  - openapi/sysdig-monitor-openapi.yml\n  - openapi/sysdig-secure-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/authentication/sysdig-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Security
- Containers
- Kubernetes
- Runtime Security
- Security
- Vulnerability Management
- Monitoring
- Observability
- CSPM
- Compliance
---
