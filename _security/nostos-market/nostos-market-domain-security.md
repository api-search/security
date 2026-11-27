---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nostos.market
  spf: true
hosts:
- cert_expires: Dec 27 22:17:58 2026 GMT
  host: nostos.market
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NOSTOS Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NOSTOS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NOSTOS
provider_slug: nostos-market
slug: nostos-market-domain-security
source_filename: nostos-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nostos.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 22:17:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nostos.market\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/nostos-market/security/nostos-market-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Retro Gaming
- Vintage Apparel
- E-Commerce
- Duluth GA
---
