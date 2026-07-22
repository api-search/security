---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: adludio.com
  spf: false
hosts:
- cert_expires: Aug 18 23:18:04 2026 GMT
  host: adludio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adludio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for adludio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: adludio
provider_slug: adludio
slug: adludio-domain-security
source_filename: adludio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adludio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:18:04 2026 GMT\n  hsts: false\ndomains:\n- domain: adludio.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adludio/refs/heads/main/security/adludio-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Advertising
- AdTech
- Mobile Advertising
- Marketing Technology
- Interactive Advertising
- Creative
---
