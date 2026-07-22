---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sprouts.com
  spf: true
hosts:
- cert_expires: Aug 30 19:48:32 2026 GMT
  host: www.sprouts.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sprouts Farmers Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sprouts Farmers Market, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sprouts Farmers Market
provider_slug: sprouts-farmers-market
slug: sprouts-farmers-market-domain-security
source_filename: sprouts-farmers-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sprouts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 19:48:32 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: sprouts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprouts-farmers-market/refs/heads/main/security/sprouts-farmers-market-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Food
- Grocery
- Organic
- Retail
- Supply Chain
---
