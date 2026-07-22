---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: edited.com
  spf: true
hosts:
- cert_expires: Sep  7 23:59:59 2026 GMT
  host: edited.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EDITED, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EDITED
provider_slug: edited
slug: edited-domain-security
source_filename: edited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edited.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: edited.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edited/refs/heads/main/security/edited-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retail
- Retail Intelligence
- Market Data
- Competitive Intelligence
- Pricing Intelligence
- Fashion
- eCommerce
- Analytics
- Data
---
