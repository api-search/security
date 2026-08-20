---
api_key_in: []
api_specs:
- filename: spot-by-netapp-audit-service-api-openapi.yml
  format: yaml
  label: Spot by NetApp Audit Service API
  slug: spot-by-netapp-audit-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-audit-service-api-openapi.yml
- filename: spot-by-netapp-create-an-api-token-api-openapi.yml
  format: yaml
  label: Spot by NetApp Create an API Token API
  slug: spot-by-netapp-create-an-api-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-create-an-api-token-api-openapi.yml
- filename: spot-by-netapp-elastigroup-aws-api-openapi.yml
  format: yaml
  label: Spot by NetApp Elastigroup AWS API
  slug: spot-by-netapp-elastigroup-aws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-elastigroup-aws-api-openapi.yml
- filename: spot-by-netapp-elastigroup-azure-spot-vms-api-openapi.yml
  format: yaml
  label: Spot by NetApp Elastigroup Azure Spot VMs API
  slug: spot-by-netapp-elastigroup-azure-spot-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-elastigroup-azure-spot-vms-api-openapi.yml
- filename: spot-by-netapp-elastigroup-gcp-api-openapi.yml
  format: yaml
  label: Spot by NetApp Elastigroup GCP API
  slug: spot-by-netapp-elastigroup-gcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-elastigroup-gcp-api-openapi.yml
- filename: spot-by-netapp-health-check-service-api-openapi.yml
  format: yaml
  label: Spot by NetApp Health Check Service API
  slug: spot-by-netapp-health-check-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-health-check-service-api-openapi.yml
- filename: spot-by-netapp-insights-service-api-openapi.yml
  format: yaml
  label: Spot by NetApp Insights Service API
  slug: spot-by-netapp-insights-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-insights-service-api-openapi.yml
- filename: spot-by-netapp-notification-subscription-service-api-openapi.yml
  format: yaml
  label: Spot by NetApp Notification Subscription Service API
  slug: spot-by-netapp-notification-subscription-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-notification-subscription-service-api-openapi.yml
- filename: spot-by-netapp-ocean-automatic-rightsizing-api-openapi.yml
  format: yaml
  label: Spot by NetApp Ocean Automatic Rightsizing API
  slug: spot-by-netapp-ocean-automatic-rightsizing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-ocean-automatic-rightsizing-api-openapi.yml
- filename: spot-by-netapp-ocean-aws-api-openapi.yml
  format: yaml
  label: Spot by NetApp Ocean AWS API
  slug: spot-by-netapp-ocean-aws-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/openapi/spot-by-netapp-ocean-aws-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Spot By Netapp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spot by NetApp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Spot by NetApp
provider_slug: spot-by-netapp
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/spot-by-netapp-openapi.yml
  type: http
slug: spot-by-netapp-authentication
source_filename: spot-by-netapp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spot-by-netapp-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/spot-by-netapp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spot-by-netapp/refs/heads/main/authentication/spot-by-netapp-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Optimization
- FinOps
- Kubernetes
- Azure
- GCP
- Cost Optimization
- Auto-Scaling
---
