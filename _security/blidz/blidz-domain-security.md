---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: blidz.com
  spf: true
hosts:
- cert_expires: Oct  2 12:59:40 2026 GMT
  host: blidz.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blidz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blidz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blidz
provider_slug: blidz
slug: blidz-domain-security
source_filename: blidz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blidz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:59:40 2026 GMT\n  hsts: false\ndomains:\n- domain: blidz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blidz/refs/heads/main/security/blidz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- E-commerce
- Shopping
- Marketplace
- Mobile
- Retail
---
