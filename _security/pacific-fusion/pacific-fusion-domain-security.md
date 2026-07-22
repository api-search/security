---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pacificfusion.com
  spf: true
hosts:
- cert_expires: Aug 28 02:36:11 2026 GMT
  host: pacificfusion.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pacific Fusion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pacific Fusion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pacific Fusion
provider_slug: pacific-fusion
slug: pacific-fusion-domain-security
source_filename: pacific-fusion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pacificfusion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 02:36:11 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: pacificfusion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pacific-fusion/refs/heads/main/security/pacific-fusion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fusion Energy
- Clean Energy
- Nuclear Fusion
- Energy
- Deep Tech
- Hardware
---
