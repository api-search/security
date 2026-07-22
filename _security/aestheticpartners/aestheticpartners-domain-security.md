---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aestheticpartners.com
  spf: true
hosts:
- cert_expires: Sep  3 15:55:19 2026 GMT
  host: aestheticpartners.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aestheticpartners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aestheticpartners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aestheticpartners
provider_slug: aestheticpartners
slug: aestheticpartners-domain-security
source_filename: aestheticpartners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aestheticpartners.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 15:55:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: aestheticpartners.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aestheticpartners/refs/heads/main/security/aestheticpartners-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Medical Aesthetics
- Healthcare
- Dermatology
- Plastic Surgery
- Practice Management
- Cosmetic
---
