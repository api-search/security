---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: weargales.com
  spf: true
hosts:
- cert_expires: Dec 27 22:29:01 2026 GMT
  host: weargales.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Weargales Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for STAND+, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: STAND+
provider_slug: weargales-com
slug: weargales-com-domain-security
source_filename: weargales-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weargales.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 22:29:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: weargales.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/weargales-com/security/weargales-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Footwear
- Recovery Shoes
- HSA/FSA Eligible
- Slip‑Resistant
- Healthcare Footwear
---
