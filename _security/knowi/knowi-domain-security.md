---
api_specs:
- filename: knowi-authentication-api-openapi.yml
  format: yaml
  label: Knowi Authentication API
  slug: knowi-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-authentication-api-openapi.yml
- filename: knowi-dashboards-api-openapi.yml
  format: yaml
  label: Knowi Dashboards API
  slug: knowi-dashboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-dashboards-api-openapi.yml
- filename: knowi-groups-api-openapi.yml
  format: yaml
  label: Knowi Groups API
  slug: knowi-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-groups-api-openapi.yml
- filename: knowi-pull-api-openapi.yml
  format: yaml
  label: Knowi Pull API
  slug: knowi-pull-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-pull-api-openapi.yml
- filename: knowi-push-api-openapi.yml
  format: yaml
  label: Knowi Push API
  slug: knowi-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-push-api-openapi.yml
- filename: knowi-users-api-openapi.yml
  format: yaml
  label: Knowi Users API
  slug: knowi-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-users-api-openapi.yml
- filename: knowi-action-management-api-api-openapi.yml
  format: yaml
  label: Knowi Action Management API
  slug: knowi-action-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-action-management-api-api-openapi.yml
- filename: knowi-alerts-api-openapi.yml
  format: yaml
  label: Knowi Alerts API
  slug: knowi-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-alerts-api-openapi.yml
- filename: knowi-authentication-management-api-api-openapi.yml
  format: yaml
  label: Knowi Authentication Management API
  slug: knowi-authentication-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-authentication-management-api-api-openapi.yml
- filename: knowi-category-management-api-api-openapi.yml
  format: yaml
  label: Knowi Category Management API
  slug: knowi-category-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-category-management-api-api-openapi.yml
- filename: knowi-datasource-management-api-api-openapi.yml
  format: yaml
  label: Knowi Datasource Management API
  slug: knowi-datasource-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-datasource-management-api-api-openapi.yml
- filename: knowi-group-management-api-api-openapi.yml
  format: yaml
  label: Knowi Group Management API
  slug: knowi-group-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-group-management-api-api-openapi.yml
- filename: knowi-kpi-management-api-api-openapi.yml
  format: yaml
  label: Knowi KPI Management API
  slug: knowi-kpi-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-kpi-management-api-api-openapi.yml
- filename: knowi-natural-language-processing-management-api-api-openapi.yml
  format: yaml
  label: Knowi Natural Language Processing Management API
  slug: knowi-natural-language-processing-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-natural-language-processing-management-api-api-openapi.yml
- filename: knowi-report-management-api-api-openapi.yml
  format: yaml
  label: Knowi Report Management API
  slug: knowi-report-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-report-management-api-api-openapi.yml
- filename: knowi-role-management-api-api-openapi.yml
  format: yaml
  label: Knowi Role Management API
  slug: knowi-role-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-role-management-api-api-openapi.yml
- filename: knowi-user-management-api-api-openapi.yml
  format: yaml
  label: Knowi User Management API
  slug: knowi-user-management-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-user-management-api-api-openapi.yml
- filename: knowi-data-sources-api-openapi.yml
  format: yaml
  label: Knowi Data Sources API
  slug: knowi-data-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/knowi/openapi/knowi-data-sources-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: knowi.com
  spf: true
hosts:
- cert_expires: Mar 15 18:17:58 2027 GMT
  host: www.knowi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 15 18:17:58 2027 GMT
  host: knowi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Knowi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Knowi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Knowi
provider_slug: knowi
slug: knowi-domain-security
source_filename: knowi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.knowi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 18:17:58 2027 GMT\n  hsts: false\n- host: knowi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 18:17:58 2027 GMT\n  hsts: false\ndomains:\n- domain: knowi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/knowi/security/knowi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI Analytics
- API Analytics
- Business Intelligence
- Data Visualization
- Embedded Analytics
- NoSQL Analytics
---
