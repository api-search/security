---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: x-rates.com
  spf: true
hosts:
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: x-rates.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Xrates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for X-Rates, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: X-Rates
provider_slug: xrates
slug: xrates-domain-security
source_filename: xrates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: x-rates.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: x-rates.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/xrates/security/xrates-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Finance
- Currency
- ExchangeRates
- API
---
