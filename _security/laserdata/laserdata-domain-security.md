---
api_specs:
- filename: laserdata-core-openapi.json
  format: json
  label: LaserData Cloud Core API
  slug: core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserdata/refs/heads/main/openapi/laserdata-core-openapi.json
- filename: laserdata-audit-openapi.json
  format: json
  label: LaserData Cloud Audit API
  slug: audit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserdata/refs/heads/main/openapi/laserdata-audit-openapi.json
- filename: laserdata-notifier-openapi.json
  format: json
  label: LaserData Cloud Notifier API
  slug: notifier
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserdata/refs/heads/main/openapi/laserdata-notifier-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: laserdata.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: laserdata.cloud
  spf: true
hosts:
- cert_expires: Sep 28 06:16:26 2026 GMT
  host: laserdata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 10:16:36 2026 GMT
  host: docs.laserdata.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 22:01:39 2026 GMT
  host: api.laserdata.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Laserdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LaserData, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: LaserData
provider_slug: laserdata
slug: laserdata-domain-security
source_filename: laserdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: laserdata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 06:16:26 2026 GMT\n  hsts: false\n- host: docs.laserdata.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 10:16:36 2026 GMT\n  hsts: false\n- host: api.laserdata.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 22:01:39 2026 GMT\n  hsts: null\ndomains:\n- domain: laserdata.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: laserdata.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laserdata/refs/heads/main/security/laserdata-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Streaming
- Message Streaming
- Event Streaming
- Data Infrastructure
- Real Time
- Apache Iggy
- Rust
- Cloud Infrastructure
- AI Agents
- Observability
- Company
---
