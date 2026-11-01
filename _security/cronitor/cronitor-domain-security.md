---
api_specs:
- filename: cronitor-groups-api-openapi.yml
  format: yaml
  label: Cronitor Groups API
  slug: cronitor-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-groups-api-openapi.yml
- filename: cronitor-notifications-api-openapi.yml
  format: yaml
  label: Cronitor Notifications API
  slug: cronitor-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-notifications-api-openapi.yml
- filename: cronitor-aggregates-api-openapi.yml
  format: yaml
  label: Cronitor Aggregates API
  slug: cronitor-aggregates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-aggregates-api-openapi.yml
- filename: cronitor-environments-api-openapi.yml
  format: yaml
  label: Cronitor Environments API
  slug: cronitor-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-environments-api-openapi.yml
- filename: cronitor-integrations-api-openapi.yml
  format: yaml
  label: Cronitor Integrations API
  slug: cronitor-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-integrations-api-openapi.yml
- filename: cronitor-issues-api-openapi.yml
  format: yaml
  label: Cronitor Issues API
  slug: cronitor-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-issues-api-openapi.yml
- filename: cronitor-keys-api-openapi.yml
  format: yaml
  label: Cronitor Keys API
  slug: cronitor-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-keys-api-openapi.yml
- filename: cronitor-maintenance-windows-api-openapi.yml
  format: yaml
  label: Cronitor Maintenance Windows API
  slug: cronitor-maintenance-windows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-maintenance-windows-api-openapi.yml
- filename: cronitor-metrics-api-openapi.yml
  format: yaml
  label: Cronitor Metrics API
  slug: cronitor-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-metrics-api-openapi.yml
- filename: cronitor-monitors-api-openapi.yml
  format: yaml
  label: Cronitor Monitors API
  slug: cronitor-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-monitors-api-openapi.yml
- filename: cronitor-search-api-openapi.yml
  format: yaml
  label: Cronitor Search API
  slug: cronitor-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-search-api-openapi.yml
- filename: cronitor-site-errors-api-openapi.yml
  format: yaml
  label: Cronitor Site Errors API
  slug: cronitor-site-errors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-site-errors-api-openapi.yml
- filename: cronitor-sites-api-openapi.yml
  format: yaml
  label: Cronitor Sites API
  slug: cronitor-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-sites-api-openapi.yml
- filename: cronitor-statuspage-components-api-openapi.yml
  format: yaml
  label: Cronitor Statuspage Components API
  slug: cronitor-statuspage-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-statuspage-components-api-openapi.yml
- filename: cronitor-statuspages-api-openapi.yml
  format: yaml
  label: Cronitor Statuspages API
  slug: cronitor-statuspages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-statuspages-api-openapi.yml
- filename: cronitor-telemetry-api-openapi.yml
  format: yaml
  label: Cronitor Telemetry API
  slug: cronitor-telemetry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cronitor/openapi/cronitor-telemetry-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cronitor.io
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: cronitor.link
  spf: false
hosts:
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: cronitor.io
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: cronitor.link
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Cronitor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cronitor, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Cronitor
provider_slug: cronitor
slug: cronitor-domain-security
source_filename: cronitor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cronitor.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: false\n- host: cronitor.link\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: cronitor.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: cronitor.link\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cronitor/security/cronitor-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Monitoring
- Cron Jobs
- Scheduled Tasks
- Alerting
- Uptime
- Telemetry
- Status Pages
- Scheduling
---
