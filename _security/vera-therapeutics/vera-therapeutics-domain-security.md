---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: veratx.com
  spf: true
hosts:
- cert_expires: Sep  9 17:04:46 2026 GMT
  host: veratx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vera Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vera Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vera Therapeutics
provider_slug: vera-therapeutics
slug: vera-therapeutics-domain-security
source_filename: vera-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: veratx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 17:04:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: veratx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vera-therapeutics/refs/heads/main/security/vera-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Life Sciences
- Biopharmaceutical
- Pharmaceuticals
- Nephrology
- Immunology
- Healthcare
---
