---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rapt.com
  spf: true
hosts:
- cert_expires: Sep 28 07:36:18 2026 GMT
  host: rapt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rapt Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RAPT Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RAPT Therapeutics
provider_slug: rapt-therapeutics
slug: rapt-therapeutics-domain-security
source_filename: rapt-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rapt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 07:36:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rapt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapt-therapeutics/refs/heads/main/security/rapt-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Biotechnology
- Pharmaceuticals
- Immunology
- Oncology
- Clinical Trials
---
