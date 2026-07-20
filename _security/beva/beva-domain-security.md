---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: beva.com
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: beva.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for beva, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: beva
provider_slug: beva
slug: beva-domain-security
source_filename: beva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: beva.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beva/refs/heads/main/security/beva-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Children
- Education
- Entertainment
- Media
- Content
- Kids Audio Video
- IP Licensing
- Open Platform
- China
---
