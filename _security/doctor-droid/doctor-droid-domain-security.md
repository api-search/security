---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: drdroid.io
  spf: true
hosts:
- cert_expires: Oct 16 14:11:16 2026 GMT
  host: drdroid.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 05:39:12 2026 GMT
  host: docs.drdroid.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 21:31:44 2026 GMT
  host: aiops.drdroid.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Doctor Droid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Doctor Droid, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Doctor Droid
provider_slug: doctor-droid
slug: doctor-droid-domain-security
source_filename: doctor-droid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: drdroid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 14:11:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.drdroid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 05:39:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: aiops.drdroid.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 21:31:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: drdroid.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doctor-droid/refs/heads/main/security/doctor-droid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- AIOps
- SRE
- Incident Response
- On-Call
- Observability
- DevOps
- Monitoring
- MCP
---
