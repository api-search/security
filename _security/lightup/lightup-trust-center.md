---
api_specs:
- filename: lightup-api-credentials-api-openapi.yml
  format: yaml
  label: Lightup API Credentials API
  slug: lightup-api-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/openapi/lightup-api-credentials-api-openapi.yml
- filename: lightup-catalogs-api-openapi.yml
  format: yaml
  label: Lightup Catalogs API
  slug: lightup-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/openapi/lightup-catalogs-api-openapi.yml
- filename: lightup-dashboard-chart-api-openapi.yml
  format: yaml
  label: Lightup Dashboard chart API
  slug: lightup-dashboard-chart-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/openapi/lightup-dashboard-chart-api-openapi.yml
- filename: lightup-datapoints-api-openapi.yml
  format: yaml
  label: Lightup Datapoints API
  slug: lightup-datapoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/openapi/lightup-datapoints-api-openapi.yml
- filename: lightup-datasources-api-openapi.yml
  format: yaml
  label: Lightup Datasources API
  slug: lightup-datasources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/openapi/lightup-datasources-api-openapi.yml
- filename: lightup-health-check-api-openapi.yml
  format: yaml
  label: Lightup Health check API
  slug: lightup-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/openapi/lightup-health-check-api-openapi.yml
- filename: lightup-incidents-api-openapi.yml
  format: yaml
  label: Lightup Incidents API
  slug: lightup-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/openapi/lightup-incidents-api-openapi.yml
- filename: lightup-integrations-api-openapi.yml
  format: yaml
  label: Lightup Integrations API
  slug: lightup-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/openapi/lightup-integrations-api-openapi.yml
- filename: lightup-metrics-api-openapi.yml
  format: yaml
  label: Lightup Metrics API
  slug: lightup-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/openapi/lightup-metrics-api-openapi.yml
- filename: lightup-monitors-api-openapi.yml
  format: yaml
  label: Lightup Monitors API
  slug: lightup-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/openapi/lightup-monitors-api-openapi.yml
- filename: lightup-users-api-openapi.yml
  format: yaml
  label: Lightup Users API
  slug: lightup-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/openapi/lightup-users-api-openapi.yml
- filename: lightup-workspaces-api-openapi.yml
  format: yaml
  label: Lightup Workspaces API
  slug: lightup-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/openapi/lightup-workspaces-api-openapi.yml
certifications:
- SOC 2 Type 2
- ISAE 3000
description: ''
kind: trust-center
layout: security
name: Lightup Trust Center
name_suffix: Trust Center
overview: Lightup maintains a public trust center documenting SOC 2 Type 2 and ISAE 3000 compliance.
provider_name: Lightup
provider_slug: lightup
slug: lightup-trust-center
source_filename: lightup-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nprobe: false\nsource: https://docs.lightup.ai/docs/key-security-features\nurl: https://docs.lightup.ai/docs/key-security-features\nnote: Lightup does not operate a dedicated trust-center subdomain (trust.lightup.ai\n  and security.lightup.ai do not resolve). Its published security and compliance posture\n  lives on the \"Key security features\" documentation page, supplemented by the legal\n  pages on the marketing site.\ncertifications:\n- SOC 2 Type 2\n- ISAE 3000\naudits:\n  third_party_pen_tests: true\n  cadence: regular\n  report_availability: recent pen-test reports available upon request\n  static_analysis: performed as part of the CI/CD pipeline\ndata_protection:\n  data_in_transit: TLS 1.2 minimum with AES-256; latest recommended secure cipher suites\n    enforced\n  data_at_rest: AES-256 via AWS-managed RDS and Redshift, encryption and periodic backup\n    snapshots always enabled (Cloud deployments)\n  source_data_copied:\
  \ false\n  source_data_note: No customer source data is copied into the Lightup environment,\n    irrespective of deployment model; checks are pushed down to the customer datasource.\n  tenancy: Single-tenant dedicated VPC per customer (Cloud deployments)\n  access_logging: All data access activity for querying DQIs, metadata or results is\n    logged.\naccess_control:\n  sso:\n  - Google SSO\n  - Okta\n  - SAML (Enterprise)\n  - Microsoft AD (Enterprise)\n  rbac: true\n  rbac_docs: https://docs.lightup.ai/docs/roles\nlegal:\n  terms_of_service: https://www.lightup.ai/terms-of-service\n  privacy_policy: https://www.lightup.ai/privacy-policy\n  dpa: https://www.lightup.ai/dpa\n  subprocessors: https://www.lightup.ai/subprocessors\n  cookie_policy: https://www.lightup.ai/cookie-policy\n  disclosure: https://www.lightup.ai/disclosure\nevidence:\n- source: https://docs.lightup.ai/docs/key-security-features\n  keywords:\n  - SOC2 Type 2\n  - ISAE 3000\n  - pen-test\n  - encryption\n  - single\
  \ tenant VPC\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/security/lightup-trust-center.yml
summary_line: SOC 2 Type 2, ISAE 3000
tags:
- Data Quality
- Data Observability
- Data Monitoring
- Anomaly Detection
- Data Engineering
- Analytics
- Incident Management
- Artificial Intelligence
- Data Governance
- Company
trust_url: https://docs.lightup.ai/docs/key-security-features
---
