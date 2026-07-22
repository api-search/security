---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: modivo.pl
  spf: true
hosts:
- cert_expires: Sep 13 18:25:33 2026 GMT
  host: modivo.pl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modivo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MODIVO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: MODIVO
provider_slug: modivo
slug: modivo-domain-security
source_filename: modivo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modivo.pl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:25:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: modivo.pl\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modivo/refs/heads/main/security/modivo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Fashion
- E-Commerce
- Retail
- Marketplace
- Retail Media
---
