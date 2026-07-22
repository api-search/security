---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dentacarts.com
  spf: true
hosts:
- cert_expires: Sep 22 19:16:05 2026 GMT
  host: dentacarts.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: X Mart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for X mart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: X mart
provider_slug: x-mart
slug: x-mart-domain-security
source_filename: x-mart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dentacarts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 19:16:05 2026 GMT\n  hsts: false\ndomains:\n- domain: dentacarts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/x-mart/refs/heads/main/security/x-mart-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Dental
- Healthcare
- Marketplace
- eCommerce
- Medical Supplies
---
