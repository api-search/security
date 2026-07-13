---
api_specs:
- filename: dremio-intelligent-lakehouse-platform-openapi.yml
  format: yaml
  label: Dremio | Intelligent Lakehouse Platform
  slug: dremio-intelligent-lakehouse-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/openapi/dremio-intelligent-lakehouse-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dremio.com
  spf: true
hosts:
- cert_expires: Sep 15 04:14:43 2026 GMT
  host: www.dremio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dremio Intelligent Lakehouse Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dremio | Intelligent Lakehouse Platform, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dremio | Intelligent Lakehouse Platform
provider_slug: dremio-intelligent-lakehouse-platform
slug: dremio-intelligent-lakehouse-platform-domain-security
source_filename: dremio-intelligent-lakehouse-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dremio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:14:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dremio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dremio-intelligent-lakehouse-platform/refs/heads/main/security/dremio-intelligent-lakehouse-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Analytics
- Lakehouse
- Apache Iceberg
- SQL
- AI
---
