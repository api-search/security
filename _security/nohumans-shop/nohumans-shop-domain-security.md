---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nohumans.shop
  spf: false
hosts:
- cert_expires: Jan 23 01:57:32 2027 GMT
  host: nohumans.shop
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: noHumansShop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for noHumansShop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: noHumansShop
provider_slug: nohumans-shop
slug: nohumans-shop-domain-security
source_filename: nohumans-shop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nohumans.shop\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 01:57:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nohumans.shop\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/nohumans-shop/security/nohumans-shop-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Affiliates
- Marketplace
- Agents
---
