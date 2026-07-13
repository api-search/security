---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tdsinc.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tdstelecom.com
  spf: true
hosts:
- cert_expires: Aug 28 10:20:13 2026 GMT
  host: www.tdsinc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: tdstelecom.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: www.arrayinc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Telephone And Data Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telephone and Data Systems, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Telephone and Data Systems
provider_slug: telephone-and-data-systems
slug: telephone-and-data-systems-domain-security
source_filename: telephone-and-data-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tdsinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 10:20:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tdstelecom.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: www.arrayinc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tdsinc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: tdstelecom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telephone-and-data-systems/refs/heads/main/security/telephone-and-data-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Broadband
- Fiber Internet
- Fortune 500
- Rural Connectivity
- Telecommunications
- Wireless Infrastructure
---
