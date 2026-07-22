---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: heygo.com
  spf: false
hosts:
- cert_expires: Aug 26 22:38:46 2026 GMT
  host: www.heygo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heygo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heygo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Heygo
provider_slug: heygo
slug: heygo-domain-security
source_filename: heygo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heygo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 22:38:46 2026 GMT\n  hsts: null\ndomains:\n- domain: heygo.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heygo/refs/heads/main/security/heygo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Live Video
- Virtual Tours
- Travel
- Streaming
- Marketplace
- Consumer
- Defunct
---
