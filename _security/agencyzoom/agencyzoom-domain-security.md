---
api_specs:
- filename: agencyzoom-authentication-api-openapi.yml
  format: yaml
  label: AgencyZoom Authentication API
  slug: agencyzoom-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-authentication-api-openapi.yml
- filename: agencyzoom-business-classifications-api-openapi.yml
  format: yaml
  label: AgencyZoom Business Classifications API
  slug: agencyzoom-business-classifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-business-classifications-api-openapi.yml
- filename: agencyzoom-configuration-and-settings-api-openapi.yml
  format: yaml
  label: AgencyZoom Configuration and Settings API
  slug: agencyzoom-configuration-and-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-configuration-and-settings-api-openapi.yml
- filename: agencyzoom-contact-management-api-openapi.yml
  format: yaml
  label: AgencyZoom Contact Management API
  slug: agencyzoom-contact-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-contact-management-api-openapi.yml
- filename: agencyzoom-customer-management-api-openapi.yml
  format: yaml
  label: AgencyZoom Customer Management API
  slug: agencyzoom-customer-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-customer-management-api-openapi.yml
- filename: agencyzoom-dashboard-api-openapi.yml
  format: yaml
  label: AgencyZoom Dashboard API
  slug: agencyzoom-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-dashboard-api-openapi.yml
- filename: agencyzoom-department-and-groups-api-openapi.yml
  format: yaml
  label: AgencyZoom Department and Groups API
  slug: agencyzoom-department-and-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-department-and-groups-api-openapi.yml
- filename: agencyzoom-lead-management-api-openapi.yml
  format: yaml
  label: AgencyZoom Lead Management API
  slug: agencyzoom-lead-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-lead-management-api-openapi.yml
- filename: agencyzoom-life-and-health-lead-management-api-openapi.yml
  format: yaml
  label: AgencyZoom Life and Health Lead Management API
  slug: agencyzoom-life-and-health-lead-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-life-and-health-lead-management-api-openapi.yml
- filename: agencyzoom-opportunity-management-api-openapi.yml
  format: yaml
  label: AgencyZoom Opportunity Management API
  slug: agencyzoom-opportunity-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-opportunity-management-api-openapi.yml
- filename: agencyzoom-pipeline-api-openapi.yml
  format: yaml
  label: AgencyZoom Pipeline API
  slug: agencyzoom-pipeline-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-pipeline-api-openapi.yml
- filename: agencyzoom-service-center-api-openapi.yml
  format: yaml
  label: AgencyZoom Service Center API
  slug: agencyzoom-service-center-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-service-center-api-openapi.yml
- filename: agencyzoom-task-management-api-openapi.yml
  format: yaml
  label: AgencyZoom Task Management API
  slug: agencyzoom-task-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-task-management-api-openapi.yml
- filename: agencyzoom-thread-api-openapi.yml
  format: yaml
  label: AgencyZoom Thread API
  slug: agencyzoom-thread-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-thread-api-openapi.yml
- filename: agencyzoom-user-management-api-openapi.yml
  format: yaml
  label: AgencyZoom User Management API
  slug: agencyzoom-user-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-user-management-api-openapi.yml
- filename: agencyzoom-v4sso-authentication-api-openapi.yml
  format: yaml
  label: AgencyZoom V4SSO Authentication API
  slug: agencyzoom-v4sso-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agencyzoom/openapi/agencyzoom-v4sso-authentication-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agencyzoom.com
  spf: true
hosts:
- cert_expires: Aug 18 21:56:07 2026 GMT
  host: agencyzoom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: app.agencyzoom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api.agencyzoom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Agencyzoom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgencyZoom, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AgencyZoom
provider_slug: agencyzoom
slug: agencyzoom-domain-security
source_filename: agencyzoom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agencyzoom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 21:56:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.agencyzoom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.agencyzoom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agencyzoom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agencyzoom/security/agencyzoom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Insurtech
- CRM
- Sales Automation
- Agency Management
- Customer Retention
---
