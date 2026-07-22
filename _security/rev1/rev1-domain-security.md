---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rev1.so
  spf: true
hosts:
- cert_expires: Sep 17 21:34:52 2026 GMT
  host: rev1.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rev1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rev1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rev1
provider_slug: rev1
slug: rev1-domain-security
source_filename: rev1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rev1.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 21:34:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rev1.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rev1/refs/heads/main/security/rev1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Manufacturing
- CAD
- Mechanical Engineering
- Artificial Intelligence
- Engineering Drawings
- GD&T
- Hardware
- Y Combinator
---
