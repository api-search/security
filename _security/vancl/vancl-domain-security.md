---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vancl.com
  spf: true
hosts:
- cert_expires: Aug 23 07:31:27 2026 GMT
  host: vancl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vancl Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VANCL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: VANCL
provider_slug: vancl
slug: vancl-domain-security
source_filename: vancl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vancl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 07:31:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vancl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vancl/refs/heads/main/security/vancl-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- eCommerce
- Apparel
- Fashion
- Retail
- China
---
