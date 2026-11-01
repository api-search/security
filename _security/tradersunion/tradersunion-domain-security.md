---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: tradersunion.com
  spf: true
hosts:
- cert_expires: Dec 18 22:21:36 2026 GMT
  host: tradersunion.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tradersunion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Traders Union, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Traders Union
provider_slug: tradersunion
slug: tradersunion-domain-security
source_filename: tradersunion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tradersunion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 22:21:36 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: tradersunion.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/tradersunion/security/tradersunion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial News
- Broker Reviews
- Trading Guides
- Market Data
- Cryptocurrency
- Foreign Exchange
- Prop Trading
---
