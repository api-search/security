---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: saama.com
  spf: true
hosts:
- cert_expires: Nov 13 01:33:30 2026 GMT
  host: www.saama.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saama, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Saama
provider_slug: saama
slug: saama-domain-security
source_filename: saama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 01:33:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: saama.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saama/refs/heads/main/security/saama-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Life Sciences
- Clinical Trials
- Clinical Data Management
- Analytics
- Artificial Intelligence
- Machine Learning
- Pharmaceuticals
- Healthcare
- Data Platform
- CDISC
---
