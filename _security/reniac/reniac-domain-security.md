---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: reniac.com
  spf: false
hosts:
- cert_expires: Oct  3 19:03:47 2026 GMT
  host: www.reniac.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reniac Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reniac, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Reniac
provider_slug: reniac
slug: reniac-domain-security
source_filename: reniac-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reniac.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 19:03:47 2026 GMT\n  hsts: false\ndomains:\n- domain: reniac.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reniac/refs/heads/main/security/reniac-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Data
- Database
- Data Acceleration
- FPGA
- Hardware Acceleration
- Infrastructure
- Performance
---
