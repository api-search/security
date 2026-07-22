---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jaysheadphones.com
  spf: true
hosts:
- cert_expires: Aug 29 19:20:06 2026 GMT
  host: jaysheadphones.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jays Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jays, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Jays
provider_slug: jays
slug: jays-domain-security
source_filename: jays-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jaysheadphones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 19:20:06 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: jaysheadphones.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jays/refs/heads/main/security/jays-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Audio
- Headphones
- Consumer Electronics
- Ecommerce
- Agent Commerce
---
