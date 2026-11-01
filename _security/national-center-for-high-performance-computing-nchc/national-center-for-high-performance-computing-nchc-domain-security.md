---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nchc.org.tw
  spf: true
hosts:
- cert_expires: Jan 27 15:59:59 2027 GMT
  host: www.nchc.org.tw
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: National Center For High Performance Computing Nchc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Center for High-performance Computing (NCHC), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: National Center for High-performance Computing (NCHC)
provider_slug: national-center-for-high-performance-computing-nchc
slug: national-center-for-high-performance-computing-nchc-domain-security
source_filename: national-center-for-high-performance-computing-nchc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nchc.org.tw\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 27 15:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nchc.org.tw\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/national-center-for-high-performance-computing-nchc/security/national-center-for-high-performance-computing-nchc-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
---
