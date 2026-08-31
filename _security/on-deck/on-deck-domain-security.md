---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: joinodf.com
  spf: true
hosts:
- cert_expires: Oct  6 18:59:16 2026 GMT
  host: joinodf.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: On Deck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for On Deck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: On Deck
provider_slug: on-deck
slug: on-deck-domain-security
source_filename: on-deck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joinodf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 18:59:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: joinodf.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/on-deck/refs/heads/main/security/on-deck-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Founder Fellowship
- Startup Accelerator
- Community
- Entrepreneurship
- Venture-Backed
- Education
---
