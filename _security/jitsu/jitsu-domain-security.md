---
api_specs:
- filename: jitsu-openapi.yml
  format: yaml
  label: Jitsu Event Ingestion API (Track / Identify / Page)
  slug: event-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitsu/refs/heads/main/openapi/jitsu-openapi.yml
- filename: jitsu-openapi.yml
  format: yaml
  label: Jitsu Bulk / Batch API
  slug: bulk-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitsu/refs/heads/main/openapi/jitsu-openapi.yml
- filename: jitsu-openapi.yml
  format: yaml
  label: Jitsu Configuration / Management
  slug: configuration-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jitsu/refs/heads/main/openapi/jitsu-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jitsu.com
  spf: true
hosts:
- cert_expires: Oct  6 03:30:27 2026 GMT
  host: jitsu.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 10:32:40 2026 GMT
  host: use.jitsu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jitsu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jitsu, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jitsu
provider_slug: jitsu
slug: jitsu-domain-security
source_filename: jitsu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jitsu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 03:30:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: use.jitsu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 10:32:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jitsu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jitsu/refs/heads/main/security/jitsu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Event Data
- CDP
- Data Pipeline
- Analytics
- Open Source
- Ingestion
---
