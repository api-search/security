---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: avalynpharma.com
  spf: true
hosts:
- cert_expires: Aug 12 23:23:22 2026 GMT
  host: avalynpharma.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Avalynpharma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avalynpharma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Avalynpharma
provider_slug: avalynpharma
slug: avalynpharma-domain-security
source_filename: avalynpharma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avalynpharma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 23:23:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: avalynpharma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avalynpharma/refs/heads/main/security/avalynpharma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Clinical Stage
- Respiratory
- Pulmonary Fibrosis
- Inhaled Therapeutics
- Life Sciences
---
