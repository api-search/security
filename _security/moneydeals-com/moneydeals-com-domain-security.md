---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: moneydeals.com
  spf: true
hosts:
- cert_expires: Feb  6 12:14:12 2027 GMT
  host: moneydeals.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MoneyDeals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MoneyDeals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MoneyDeals
provider_slug: moneydeals-com
slug: moneydeals-com-domain-security
source_filename: moneydeals-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moneydeals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 12:14:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: moneydeals.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/moneydeals-com/security/moneydeals-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Tech Deals
- E-Commerce
- Affiliates
- Consumer Electronics
- US Market
---
