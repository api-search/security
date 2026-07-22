---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: columnar.tech
  spf: true
hosts:
- cert_expires: Sep 23 21:08:05 2026 GMT
  host: columnar.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Columnar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Columnar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Columnar
provider_slug: columnar
slug: columnar-domain-security
source_filename: columnar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: columnar.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:08:05 2026 GMT\n  hsts: false\ndomains:\n- domain: columnar.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/columnar/refs/heads/main/security/columnar-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Data
- ADBC
- Apache Arrow
- Database Connectivity
- Drivers
- CLI
- DuckDB
- Open Source
- Agent Skills
---
