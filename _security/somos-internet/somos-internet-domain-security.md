---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: somosinternet.com
  spf: true
hosts:
- cert_expires: Sep 23 13:20:43 2026 GMT
  host: www.somosinternet.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Somos Internet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Somos Internet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Somos Internet
provider_slug: somos-internet
slug: somos-internet-domain-security
source_filename: somos-internet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.somosinternet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 13:20:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: somosinternet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/somos-internet/refs/heads/main/security/somos-internet-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Telecom
- Internet Service Provider
- Fiber Optic
- Broadband
- Connectivity
- Colombia
- Latin America
---
