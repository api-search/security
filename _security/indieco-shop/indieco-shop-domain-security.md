---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: indieco.shop
  spf: true
hosts:
- cert_expires: Jan 17 16:12:08 2027 GMT
  host: indieco.shop
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: indieco-shop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for indieco-shop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: indieco-shop
provider_slug: indieco-shop
slug: indieco-shop-domain-security
source_filename: indieco-shop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: indieco.shop\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 16:12:08 2027 GMT\n  hsts: null\ndomains:\n- domain: indieco.shop\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/indieco-shop/security/indieco-shop-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
