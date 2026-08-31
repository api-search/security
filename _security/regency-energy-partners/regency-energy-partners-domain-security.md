---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: regencyenergy.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: energytransfer.com
  spf: true
hosts:
- cert_expires: Jan 10 10:12:13 2027 GMT
  host: www.regencyenergy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 06:21:52 2026 GMT
  host: ir.energytransfer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Regency Energy Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for regency-energy-partners, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: regency-energy-partners
provider_slug: regency-energy-partners
slug: regency-energy-partners-domain-security
source_filename: regency-energy-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.regencyenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 10:12:13 2027 GMT\n  hsts: null\n- host: ir.energytransfer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 06:21:52 2026 GMT\n  hsts: null\ndomains:\n- domain: regencyenergy.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: energytransfer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regency-energy-partners/refs/heads/main/security/regency-energy-partners-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Midstream
- Natural Gas
- Energy
- Master Limited Partnership
- Oil And Gas
- Pipeline
- Gathering And Processing
---
