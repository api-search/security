---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bellwether.markets
  spf: false
hosts:
- cert_expires: Jan 28 00:22:49 2027 GMT
  host: bellwether.markets
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bellwether Markets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bellwether-markets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: bellwether-markets
provider_slug: bellwether-markets
slug: bellwether-markets-domain-security
source_filename: bellwether-markets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bellwether.markets\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 00:22:49 2027 GMT\n  hsts: null\ndomains:\n- domain: bellwether.markets\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bellwether-markets/security/bellwether-markets-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Prediction-Market
- API
- FinTech
- Data-Aggregation
---
