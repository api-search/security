---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-managed-prometheus-tags-api-openapi.yml
  format: yaml
  label: Amazon Managed Service for Prometheus Tags API
  slug: amazon-managed-prometheus-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-managed-prometheus/openapi/amazon-managed-prometheus-tags-api-openapi.yml
- filename: amazon-managed-prometheus-workspaces-api-openapi.yml
  format: yaml
  label: Amazon Managed Service for Prometheus Workspaces API
  slug: amazon-managed-prometheus-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-managed-prometheus/openapi/amazon-managed-prometheus-workspaces-api-openapi.yml
- filename: amazon-managed-prometheus-anomalydetectors-api-openapi.yml
  format: yaml
  label: Amazon Managed Service for Prometheus Managed Prometheus Anomalydetectors API
  slug: amazon-managed-prometheus-anomalydetectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-managed-prometheus/openapi/amazon-managed-prometheus-anomalydetectors-api-openapi.yml
- filename: amazon-managed-prometheus-logging-api-openapi.yml
  format: yaml
  label: Amazon Managed Service for Prometheus Managed Prometheus Logging API
  slug: amazon-managed-prometheus-logging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-managed-prometheus/openapi/amazon-managed-prometheus-logging-api-openapi.yml
- filename: amazon-managed-prometheus-logging-configuration-api-openapi.yml
  format: yaml
  label: Amazon Managed Service for Prometheus Managed Prometheus Logging Configuration API
  slug: amazon-managed-prometheus-logging-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-managed-prometheus/openapi/amazon-managed-prometheus-logging-configuration-api-openapi.yml
- filename: amazon-managed-prometheus-operations-api-openapi.yml
  format: yaml
  label: Amazon Managed Service for Prometheus Managed Prometheus Operations API
  slug: amazon-managed-prometheus-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-managed-prometheus/openapi/amazon-managed-prometheus-operations-api-openapi.yml
- filename: amazon-managed-prometheus-policy-api-openapi.yml
  format: yaml
  label: Amazon Managed Service for Prometheus Managed Prometheus Policy API
  slug: amazon-managed-prometheus-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-managed-prometheus/openapi/amazon-managed-prometheus-policy-api-openapi.yml
- filename: amazon-managed-prometheus-scrapers-api-openapi.yml
  format: yaml
  label: Amazon Managed Service for Prometheus Managed Prometheus Scrapers API
  slug: amazon-managed-prometheus-scrapers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-managed-prometheus/openapi/amazon-managed-prometheus-scrapers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Managed Prometheus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon Managed Service for Prometheus secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-managed-prometheus-openapi-original.yaml
  type: apiKey
slug: amazon-managed-prometheus-authentication
source_filename: amazon-managed-prometheus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-managed-prometheus-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-managed-prometheus-openapi-original.yaml\n"
source_yaml_url: https://artifacts.apis.io/amazon-managed-prometheus/authentication/amazon-managed-prometheus-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Containers
- Monitoring
- Observability
- Prometheus
---
