---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: chupps.com
  spf: true
hosts:
- cert_expires: Nov 18 19:45:01 2026 GMT
  host: chupps.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chupps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chupps, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Chupps
provider_slug: chupps
slug: chupps-domain-security
source_filename: chupps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chupps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 19:45:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: chupps.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chupps/refs/heads/main/security/chupps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Footwear
- Sliders
- Sandals
- Clogs
- Flip‑Flops
- Biodegradable
- Men
- Women
---
