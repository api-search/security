---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-emr-clusters-api-openapi.yml
  format: yaml
  label: Amazon EMR Clusters API
  slug: amazon-emr-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-clusters-api-openapi.yml
- filename: amazon-emr-auto-termination-policy-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Auto Termination Policy API
  slug: amazon-emr-auto-termination-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-auto-termination-policy-api-openapi.yml
- filename: amazon-emr-instance-fleet-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Instance Fleet API
  slug: amazon-emr-instance-fleet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-instance-fleet-api-openapi.yml
- filename: amazon-emr-instance-group-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Instance Group API
  slug: amazon-emr-instance-group-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-instance-group-api-openapi.yml
- filename: amazon-emr-managed-scaling-policy-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Managed Scaling Policy API
  slug: amazon-emr-managed-scaling-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-managed-scaling-policy-api-openapi.yml
- filename: amazon-emr-notebook-execution-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Notebook Execution API
  slug: amazon-emr-notebook-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-notebook-execution-api-openapi.yml
- filename: amazon-emr-operations-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Operations API
  slug: amazon-emr-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-operations-api-openapi.yml
- filename: amazon-emr-security-configuration-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Security Configuration API
  slug: amazon-emr-security-configuration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-security-configuration-api-openapi.yml
- filename: amazon-emr-session-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Session API
  slug: amazon-emr-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-session-api-openapi.yml
- filename: amazon-emr-step-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Step API
  slug: amazon-emr-step-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-step-api-openapi.yml
- filename: amazon-emr-studio-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Studio API
  slug: amazon-emr-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-studio-api-openapi.yml
- filename: amazon-emr-studio-session-mapping-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Studio Session Mapping API
  slug: amazon-emr-studio-session-mapping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-studio-session-mapping-api-openapi.yml
- filename: amazon-emr-applications-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Applications API
  slug: amazon-emr-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-applications-api-openapi.yml
- filename: amazon-emr-endpoints-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Endpoints API
  slug: amazon-emr-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-endpoints-api-openapi.yml
- filename: amazon-emr-jobruns-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Jobruns API
  slug: amazon-emr-jobruns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-jobruns-api-openapi.yml
- filename: amazon-emr-tags-api-openapi.yml
  format: yaml
  label: Amazon EMR Emr Tags API
  slug: amazon-emr-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-tags-api-openapi.yml
- filename: amazon-emr-job-templates-api-openapi.yml
  format: yaml
  label: Amazon EMR Job Templates API
  slug: amazon-emr-job-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-job-templates-api-openapi.yml
- filename: amazon-emr-virtual-clusters-api-openapi.yml
  format: yaml
  label: Amazon EMR Virtual Clusters API
  slug: amazon-emr-virtual-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-emr/openapi/amazon-emr-virtual-clusters-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon EMR Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon EMR secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon EMR
provider_slug: amazon-emr
scheme_count: 1
schemes:
- description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256 signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token for temporary credentials). Not a bearer token.
  in: header
  name: sigv4
  parameter: Authorization
  sources:
  - openapi/amazon-emr-applications-api-openapi.yml
  - openapi/amazon-emr-auto-termination-policy-api-openapi.yml
  - openapi/amazon-emr-clusters-api-openapi.yml
  - openapi/amazon-emr-endpoints-api-openapi.yml
  - openapi/amazon-emr-instance-fleet-api-openapi.yml
  - openapi/amazon-emr-instance-group-api-openapi.yml
  - openapi/amazon-emr-jobruns-api-openapi.yml
  - openapi/amazon-emr-jobtemplates-api-openapi.yml
  - openapi/amazon-emr-managed-scaling-policy-api-openapi.yml
  - openapi/amazon-emr-notebook-execution-api-openapi.yml
  - openapi/amazon-emr-operations-api-openapi.yml
  - openapi/amazon-emr-security-configuration-api-openapi.yml
  - openapi/amazon-emr-session-api-openapi.yml
  - openapi/amazon-emr-step-api-openapi.yml
  - openapi/amazon-emr-studio-api-openapi.yml
  - openapi/amazon-emr-studio-session-mapping-api-openapi.yml
  - openapi/amazon-emr-tags-api-openapi.yml
  - openapi/amazon-emr-virtualclusters-api-openapi.yml
  type: apiKey
slug: amazon-emr-authentication
source_filename: amazon-emr-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/amazon-emr-applications-api-openapi.yml, openapi/amazon-emr-auto-termination-policy-api-openapi.yml,\n  openapi/amazon-emr-clusters-api-openapi.yml, openapi/amazon-emr-endpoints-api-openapi.yml,\n  openapi/amazon-emr-instance-fleet-api-openapi.yml, openapi/amazon-emr-instance-group-api-openapi.yml,\n  openapi/amazon-emr-jobruns-api-openapi.yml, openapi/amazon-emr-jobtemplates-api-openapi.yml,\n  openapi/amazon-emr-managed-scaling-policy-api-openapi.yml, openapi/amazon-emr-notebook-execution-api-openapi.yml,\n  openapi/amazon-emr-operations-api-openapi.yml, openapi/amazon-emr-security-configuration-api-openapi.yml\n  ...\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: sigv4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4. The Authorization header carries an AWS4-HMAC-SHA256\n    signature over the canonical request, with X-Amz-Date (and X-Amz-Security-Token\
  \ for temporary\n    credentials). Not a bearer token.\n  sources:\n  - openapi/amazon-emr-applications-api-openapi.yml\n  - openapi/amazon-emr-auto-termination-policy-api-openapi.yml\n  - openapi/amazon-emr-clusters-api-openapi.yml\n  - openapi/amazon-emr-endpoints-api-openapi.yml\n  - openapi/amazon-emr-instance-fleet-api-openapi.yml\n  - openapi/amazon-emr-instance-group-api-openapi.yml\n  - openapi/amazon-emr-jobruns-api-openapi.yml\n  - openapi/amazon-emr-jobtemplates-api-openapi.yml\n  - openapi/amazon-emr-managed-scaling-policy-api-openapi.yml\n  - openapi/amazon-emr-notebook-execution-api-openapi.yml\n  - openapi/amazon-emr-operations-api-openapi.yml\n  - openapi/amazon-emr-security-configuration-api-openapi.yml\n  - openapi/amazon-emr-session-api-openapi.yml\n  - openapi/amazon-emr-step-api-openapi.yml\n  - openapi/amazon-emr-studio-api-openapi.yml\n  - openapi/amazon-emr-studio-session-mapping-api-openapi.yml\n  - openapi/amazon-emr-tags-api-openapi.yml\n  - openapi/amazon-emr-virtualclusters-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-emr/authentication/amazon-emr-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Amazon Web Services
- Analytics
- Apache Spark
- Big Data
- Data Processing
- Hadoop
---
