---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: comerica.com
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: www.comerica.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Comerica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comerica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Comerica
provider_slug: comerica
slug: comerica-domain-security
source_filename: comerica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.comerica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: comerica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comerica/refs/heads/main/security/comerica-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Commercial Banking
- Financial Services
- Retail Banking
- Wealth Management
- Fortune 1000
---
