---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: earningswave.com
  spf: true
hosts:
- cert_expires: Jan 16 09:10:43 2027 GMT
  host: earningswave.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Earningswave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EarningsWave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EarningsWave
provider_slug: earningswave
slug: earningswave-domain-security
source_filename: earningswave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: earningswave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 09:10:43 2027 GMT\n  hsts: null\ndomains:\n- domain: earningswave.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/earningswave/security/earningswave-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Finance
- Data
- Earnings
---
