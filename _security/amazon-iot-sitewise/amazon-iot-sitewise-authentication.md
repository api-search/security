---
api_key_in:
- header
api_specs:
- filename: amazon-iot-sitewise-access-policies-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Access Policies API
  slug: amazon-iot-sitewise-access-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-access-policies-api-openapi.yml
- filename: amazon-iot-sitewise-asset-models-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Asset Models API
  slug: amazon-iot-sitewise-asset-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-asset-models-api-openapi.yml
- filename: amazon-iot-sitewise-assets-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Assets API
  slug: amazon-iot-sitewise-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-assets-api-openapi.yml
- filename: amazon-iot-sitewise-configuration-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Configuration API
  slug: amazon-iot-sitewise-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-configuration-api-openapi.yml
- filename: amazon-iot-sitewise-dashboards-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Dashboards API
  slug: amazon-iot-sitewise-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-dashboards-api-openapi.yml
- filename: amazon-iot-sitewise-dashboards-projectid-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Dashboards#projectId API
  slug: amazon-iot-sitewise-dashboards-projectid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-dashboards-projectid-api-openapi.yml
- filename: amazon-iot-sitewise-gateways-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Gateways API
  slug: amazon-iot-sitewise-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-gateways-api-openapi.yml
- filename: amazon-iot-sitewise-jobs-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Jobs API
  slug: amazon-iot-sitewise-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-jobs-api-openapi.yml
- filename: amazon-iot-sitewise-logging-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Logging API
  slug: amazon-iot-sitewise-logging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-logging-api-openapi.yml
- filename: amazon-iot-sitewise-portals-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Portals API
  slug: amazon-iot-sitewise-portals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-portals-api-openapi.yml
- filename: amazon-iot-sitewise-projects-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Projects API
  slug: amazon-iot-sitewise-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-projects-api-openapi.yml
- filename: amazon-iot-sitewise-projects-portalid-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Projects#portalId API
  slug: amazon-iot-sitewise-projects-portalid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-projects-portalid-api-openapi.yml
- filename: amazon-iot-sitewise-properties-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Properties API
  slug: amazon-iot-sitewise-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-properties-api-openapi.yml
- filename: amazon-iot-sitewise-tags-resourcearn-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Tags#resourceArn API
  slug: amazon-iot-sitewise-tags-resourcearn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-tags-resourcearn-api-openapi.yml
- filename: amazon-iot-sitewise-tags-resourcearn-tagkeys-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Tags#resourceArn&tagKeys API
  slug: amazon-iot-sitewise-tags-resourcearn-tagkeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-tags-resourcearn-tagkeys-api-openapi.yml
- filename: amazon-iot-sitewise-timeseries-api-openapi.yml
  format: yaml
  label: Amazon IoT SiteWise Timeseries API
  slug: amazon-iot-sitewise-timeseries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/openapi/amazon-iot-sitewise-timeseries-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Iot Sitewise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon IoT SiteWise secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon IoT SiteWise
provider_slug: amazon-iot-sitewise
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-iot-sitewise-openapi-original.yml
  type: apiKey
slug: amazon-iot-sitewise-authentication
source_filename: amazon-iot-sitewise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-iot-sitewise-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-iot-sitewise-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-iot-sitewise/refs/heads/main/authentication/amazon-iot-sitewise-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Asset Management
- Industrial IoT
- IoT
- Time Series Data
---
