---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ai2sql.io
  spf: true
hosts:
- cert_expires: Jan  9 14:49:00 2027 GMT
  host: ai2sql.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI2SQL Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI2SQL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: AI2SQL
provider_slug: ai2sql-io
slug: ai2sql-io-domain-security
source_filename: ai2sql-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai2sql.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 14:49:00 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ai2sql.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ai2sql-io/security/ai2sql-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- SQL
- Database
- Automation
- No-Code
- Developer Tools
---
