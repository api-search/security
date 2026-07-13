---
api_specs:
- filename: holistics-openapi.yml
  format: yaml
  label: Holistics Data Schedules & Jobs API
  slug: holistics-data-schedules-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/openapi/holistics-openapi.yml
- filename: holistics-openapi.yml
  format: yaml
  label: Holistics Dashboards & Reports API
  slug: holistics-dashboards-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/openapi/holistics-openapi.yml
- filename: holistics-openapi.yml
  format: yaml
  label: Holistics Export API
  slug: holistics-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/openapi/holistics-openapi.yml
- filename: holistics-openapi.yml
  format: yaml
  label: Holistics Users & Permissions API
  slug: holistics-users-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/openapi/holistics-openapi.yml
- filename: holistics-openapi.yml
  format: yaml
  label: Holistics Embedded Analytics API
  slug: holistics-embedded-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/openapi/holistics-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: holistics.io
  spf: true
hosts:
- cert_expires: Aug 19 21:27:02 2026 GMT
  host: www.holistics.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 21:27:02 2026 GMT
  host: docs-v2.holistics.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 21:27:02 2026 GMT
  host: secure.holistics.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Holistics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Holistics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Holistics
provider_slug: holistics
slug: holistics-domain-security
source_filename: holistics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.holistics.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 21:27:02 2026 GMT\n  hsts: false\n- host: docs-v2.holistics.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 21:27:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: secure.holistics.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 21:27:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: holistics.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holistics/refs/heads/main/security/holistics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Business Intelligence
- Analytics
- Self-Service BI
- Data Modeling
- Embedded Analytics
---
