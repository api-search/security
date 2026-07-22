---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fabfitfun.com
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: fabfitfun.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fabfitfun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FabFitFun, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FabFitFun
provider_slug: fabfitfun
slug: fabfitfun-domain-security
source_filename: fabfitfun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fabfitfun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fabfitfun.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fabfitfun/refs/heads/main/security/fabfitfun-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Subscription
- E-Commerce
- Retail
- Consumer
- Beauty
- Lifestyle
- Direct-to-Consumer
---
