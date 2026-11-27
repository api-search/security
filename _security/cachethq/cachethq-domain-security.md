---
api_specs:
- filename: cachethq-cachet-api-openapi.yml
  format: yaml
  label: Cachet Cachet API
  slug: cachethq-cachet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-cachet-api-openapi.yml
- filename: cachethq-component-groups-api-openapi.yml
  format: yaml
  label: Cachet Component Groups API
  slug: cachethq-component-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-component-groups-api-openapi.yml
- filename: cachethq-components-api-openapi.yml
  format: yaml
  label: Cachet Components API
  slug: cachethq-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-components-api-openapi.yml
- filename: cachethq-incident-templates-api-openapi.yml
  format: yaml
  label: Cachet Incident Templates API
  slug: cachethq-incident-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-incident-templates-api-openapi.yml
- filename: cachethq-incident-updates-api-openapi.yml
  format: yaml
  label: Cachet Incident Updates API
  slug: cachethq-incident-updates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-incident-updates-api-openapi.yml
- filename: cachethq-incidents-api-openapi.yml
  format: yaml
  label: Cachet Incidents API
  slug: cachethq-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-incidents-api-openapi.yml
- filename: cachethq-metric-points-api-openapi.yml
  format: yaml
  label: Cachet Metric Points API
  slug: cachethq-metric-points-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-metric-points-api-openapi.yml
- filename: cachethq-metrics-api-openapi.yml
  format: yaml
  label: Cachet Metrics API
  slug: cachethq-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-metrics-api-openapi.yml
- filename: cachethq-schedule-updates-api-openapi.yml
  format: yaml
  label: Cachet Schedule Updates API
  slug: cachethq-schedule-updates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-schedule-updates-api-openapi.yml
- filename: cachethq-schedules-api-openapi.yml
  format: yaml
  label: Cachet Schedules API
  slug: cachethq-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-schedules-api-openapi.yml
- filename: cachethq-subscribers-api-openapi.yml
  format: yaml
  label: Cachet Subscribers API
  slug: cachethq-subscribers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cachethq/openapi/cachethq-subscribers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cachethq.io
  spf: true
hosts:
- cert_expires: Feb  6 11:19:18 2027 GMT
  host: cachethq.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cachet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cachet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cachet
provider_slug: cachethq
slug: cachethq-domain-security
source_filename: cachethq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cachethq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 11:19:18 2027 GMT\n  hsts: false\ndomains:\n- domain: cachethq.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cachethq/security/cachethq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Open Source
- Status Pages
- Incident Management
- Monitoring
---
