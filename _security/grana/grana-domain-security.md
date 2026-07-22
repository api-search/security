---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: grana.com
  spf: false
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: grana.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Grana
provider_slug: grana
slug: grana-domain-security
source_filename: grana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: grana.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grana/refs/heads/main/security/grana-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fashion
- Apparel
- E-Commerce
- Direct-to-Consumer
- Retail
- Consumer
- Hong Kong
---
