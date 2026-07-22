---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vanillasteel.com
  spf: true
hosts:
- cert_expires: Oct 15 23:40:49 2026 GMT
  host: vanillasteel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vanilla Steel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vanilla Steel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vanilla Steel
provider_slug: vanilla-steel
slug: vanilla-steel-domain-security
source_filename: vanilla-steel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vanillasteel.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 23:40:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vanillasteel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanilla-steel/refs/heads/main/security/vanilla-steel-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Steel
- Metals
- Marketplace
- Trading
- B2B
- Procurement
- RFQ
- Logistics
---
