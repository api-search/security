---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ottertune.com
  spf: true
hosts:
- cert_expires: Oct  4 23:23:51 2026 GMT
  host: ottertune.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ottertune Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OtterTune, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OtterTune
provider_slug: ottertune
slug: ottertune-domain-security
source_filename: ottertune-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ottertune.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:23:51 2026 GMT\n  hsts: false\ndomains:\n- domain: ottertune.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ottertune/refs/heads/main/security/ottertune-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Big Data
- Database
- Database Optimization
- Machine Learning
- PostgreSQL
- MySQL
- Defunct
---
