---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nodajimarket.com
  spf: true
hosts:
- cert_expires: Feb 14 04:20:37 2027 GMT
  host: nodajimarket.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: NodajiMarket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NodajiMarket, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: NodajiMarket
provider_slug: nodajimarket-com
slug: nodajimarket-com-domain-security
source_filename: nodajimarket-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nodajimarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 04:20:37 2027 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: nodajimarket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nodajimarket-com/security/nodajimarket-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketplace
- E-Commerce
- Korean
- Global
- Artisans
---
