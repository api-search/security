---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: belk.com
  spf: true
hosts:
- cert_expires: Mar 24 20:00:12 2027 GMT
  host: www.belk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Belk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Belk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Belk
provider_slug: belk
slug: belk-domain-security
source_filename: belk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.belk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 24 20:00:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: belk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/belk/refs/heads/main/security/belk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apparel
- Beauty
- Department Store
- E-Commerce
- Fashion
- Home Goods
- Jewelry
- Marketplace
- Retail
- Southeastern US
---
