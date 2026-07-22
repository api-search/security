---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fanli.com
  spf: true
hosts:
- cert_expires: Nov 27 08:31:01 2026 GMT
  host: fanli.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fanli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fanli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: fanli
provider_slug: fanli
slug: fanli-domain-security
source_filename: fanli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fanli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 08:31:01 2026 GMT\n  hsts: false\ndomains:\n- domain: fanli.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fanli/refs/heads/main/security/fanli-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Cashback
- Shopping
- Rewards
- Coupons
- Retail
- China
---
