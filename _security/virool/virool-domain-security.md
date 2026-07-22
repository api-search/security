---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: virool.com
  spf: true
hosts:
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: virool.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Virool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virool, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Virool
provider_slug: virool
slug: virool-domain-security
source_filename: virool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: virool.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: virool.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virool/refs/heads/main/security/virool-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Advertising
- Video Advertising
- Video
- AdTech
- Marketing
- Brand
- Media
---
