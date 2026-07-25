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
description: ''
domains:
- caa:
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: lightup.ai
  spf: true
hosts:
- cert_expires: Sep 18 04:18:11 2026 GMT
  host: www.lightup.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 04:01:35 2026 GMT
  host: docs.lightup.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 06:42:48 2026 GMT
  host: app.demo.lightup.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightup, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Lightup
provider_slug: lightup
slug: lightup-domain-security
source_filename: lightup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lightup.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 04:18:11 2026 GMT\n  hsts: false\n- host: docs.lightup.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:01:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.demo.lightup.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:42:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lightup.ai\n  dnssec: true\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightup/refs/heads/main/security/lightup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
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
---
