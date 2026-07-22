---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: edisonscientific.com
  spf: true
hosts:
- cert_expires: Oct 14 08:18:12 2026 GMT
  host: edisonscientific.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edison Scientific Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edison Scientific, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Edison Scientific
provider_slug: edison-scientific
slug: edison-scientific-domain-security
source_filename: edison-scientific-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edisonscientific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 08:18:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: edisonscientific.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edison-scientific/refs/heads/main/security/edison-scientific-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Artificial Intelligence
- Drug Discovery
- Biopharma
- Life Sciences
- Research
- R&D
- Machine Learning
---
