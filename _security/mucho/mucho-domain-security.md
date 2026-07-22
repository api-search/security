---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mucho.asia
  spf: true
hosts:
- cert_expires: Sep 18 02:32:20 2026 GMT
  host: mucho.asia
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mucho Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mucho, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: mucho
provider_slug: mucho
slug: mucho-domain-security
source_filename: mucho-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mucho.asia\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 02:32:20 2026 GMT\n  hsts: false\ndomains:\n- domain: mucho.asia\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mucho/refs/heads/main/security/mucho-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Social Commerce
- E-Commerce
- Group Buying
- Retail
- Indonesia
- Mobile Shopping
- Defunct
---
