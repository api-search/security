---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fastmarkets.com
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: www.fastmarkets.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fastmarkets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fastmarkets, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fastmarkets
provider_slug: fastmarkets
slug: fastmarkets-domain-security
source_filename: fastmarkets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fastmarkets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: fastmarkets.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fastmarkets/security/fastmarkets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Price Reporting
- Commodity Data
- Market Forecasts
- Risk Management
- Consulting
- Event
- Platform
---
