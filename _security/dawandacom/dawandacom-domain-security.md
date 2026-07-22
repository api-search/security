---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dawanda.com
  spf: true
hosts:
- cert_expires: Oct  4 04:59:11 2026 GMT
  host: www.dawanda.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dawandacom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DaWanda.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: DaWanda.com
provider_slug: dawandacom
slug: dawandacom-domain-security
source_filename: dawandacom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dawanda.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 04:59:11 2026 GMT\n  hsts: null\ndomains:\n- domain: dawanda.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dawandacom/refs/heads/main/security/dawandacom-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Marketplace
- E-Commerce
- Handmade
- Germany
- Defunct
---
