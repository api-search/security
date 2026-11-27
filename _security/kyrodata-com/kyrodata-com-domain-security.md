---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: kyrodata.com
  spf: true
hosts:
- cert_expires: Jan 14 18:59:18 2027 GMT
  host: kyrodata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kyrodata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kyrodata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Kyrodata
provider_slug: kyrodata-com
slug: kyrodata-com-domain-security
source_filename: kyrodata-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kyrodata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 18:59:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kyrodata.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kyrodata-com/security/kyrodata-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Data
- Commodities
- Forecasting
- Trade Intelligence
- Brazil
---
