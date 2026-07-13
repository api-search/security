---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wsfsbank.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bmt.com
  spf: true
hosts:
- cert_expires: Aug 19 05:59:58 2026 GMT
  host: www.wsfsbank.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 10:27:21 2026 GMT
  host: www.bmt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wsfs Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WSFS Financial, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: WSFS Financial
provider_slug: wsfs-financial
slug: wsfs-financial-domain-security
source_filename: wsfs-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wsfsbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 05:59:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.bmt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 10:27:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: wsfsbank.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: bmt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wsfs-financial/refs/heads/main/security/wsfs-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Wealth Management
- Trust Services
- Cash Logistics
- Commercial Banking
---
