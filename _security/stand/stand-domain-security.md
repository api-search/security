---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: standshoes.com
  spf: true
hosts:
- cert_expires: Sep 15 18:12:32 2026 GMT
  host: www.standshoes.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stand Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for STAND+, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: STAND+
provider_slug: stand
slug: stand-domain-security
source_filename: stand-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.standshoes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 18:12:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: standshoes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stand/refs/heads/main/security/stand-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Footwear
- Consumer Products
- E-Commerce
- Health
- Wearables
- Recovery
- Retail
---
