---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ahana.io
  spf: true
hosts:
- cert_expires: Aug 17 11:54:35 2026 GMT
  host: ahana.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ahana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ahana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ahana
provider_slug: ahana
slug: ahana-domain-security
source_filename: ahana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ahana.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 11:54:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ahana.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ahana/refs/heads/main/security/ahana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Presto
- PrestoDB
- Data Lakehouse
- Analytics
- SQL Query Engine
- Open Source
- Data
- Acquired
---
