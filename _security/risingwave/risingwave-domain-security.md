---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: risingwave.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: risingwave.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 00:17:02 2026 GMT
  host: docs.risingwave.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Risingwave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RisingWave, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RisingWave
provider_slug: risingwave
slug: risingwave-domain-security
source_filename: risingwave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: risingwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n- host: docs.risingwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:17:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: risingwave.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/risingwave/refs/heads/main/security/risingwave-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Streaming
- SQL
- Database
- Real-Time
- Kafka
- Materialized Views
- PostgreSQL
- Apache Iceberg
---
