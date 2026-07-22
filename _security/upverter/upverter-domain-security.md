---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: upverter.com
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: upverter.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Upverter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Upverter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Upverter
provider_slug: upverter
slug: upverter-domain-security
source_filename: upverter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upverter.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: upverter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/upverter/refs/heads/main/security/upverter-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Hardware
- Electronics
- PCB Design
- EDA
- Collaboration
---
