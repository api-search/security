---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: insmed.com
  spf: true
hosts:
- cert_expires: Sep  6 19:26:54 2026 GMT
  host: www.insmed.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Insmed Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insmed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Insmed
provider_slug: insmed
slug: insmed-domain-security
source_filename: insmed-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.insmed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 19:26:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: insmed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insmed/refs/heads/main/security/insmed-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotech
- Biopharmaceutical
- Pharmaceuticals
- Healthcare
- Rare Disease
- Clinical Trials
- Life Sciences
---
