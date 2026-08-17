---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: webloyalty.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: webloyalty.co.uk
  method: probed-by-hand
  spf: true
hosts:
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: webloyalty.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  5 23:59:59 2027 GMT
  cert_issuer: Amazon RSA 2048 M01
  host: webloyalty.co.uk
  hsts: false
  https: true
  method: probed-by-hand
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Webloyalty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Webloyalty, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Webloyalty
provider_slug: webloyalty
slug: webloyalty-domain-security
source_filename: webloyalty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  webloyalty.co.uk was probed by hand on 2026-08-13 because it is the host that\n  actually serves Webloyalty's programmable surface (the OAuth authorization\n  server and the MCP endpoint), and it is not reachable from an apis[] entry —\n  the profile has none. A later automated run of probe-domain-security.py will\n  regenerate this file from apis.yml hosts only and may drop that row.\nhosts:\n- host: webloyalty.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: false\n- host: webloyalty.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  cert_issuer: Amazon RSA 2048 M01\n  hsts: false\n  method: probed-by-hand\ndomains:\n- domain: webloyalty.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: webloyalty.co.uk\n  dnssec: false\n  caa: []\n\
  \  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  method: probed-by-hand\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webloyalty/refs/heads/main/security/webloyalty-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Loyalty
- Rewards
- Ecommerce
- Customer Engagement
- Marketing
- Retail
- Cashback
---
