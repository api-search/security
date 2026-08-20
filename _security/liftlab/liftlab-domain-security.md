---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: liftlab.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: liftlab.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 03:44:37 2026 GMT
  host: connect.liftlab.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liftlab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiftLab, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LiftLab
provider_slug: liftlab
slug: liftlab-domain-security
source_filename: liftlab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liftlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: false\n- host: connect.liftlab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:44:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: liftlab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liftlab/refs/heads/main/security/liftlab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Marketing
- Marketing Measurement
- Marketing Mix Modeling
- Incrementality
- Analytics
- MarTech
- Attribution
- Budget Optimization
- Data Science
- Software-as-a-Service
---
