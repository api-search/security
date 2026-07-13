---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wproxy.org
  spf: false
hosts:
- cert_expires: Sep 29 18:35:20 2026 GMT
  host: wproxy.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Whistle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Whistle, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Whistle
provider_slug: whistle
slug: whistle-domain-security
source_filename: whistle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wproxy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:35:20 2026 GMT\n  hsts: false\ndomains:\n- domain: wproxy.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/whistle/refs/heads/main/security/whistle-domain-security.yml
summary_line: TLSv1.3
tags:
- Debugging Proxy
- Proxy
- Network Debugging
- HTTP
- HTTPS
- WebSocket
- Developer Tools
---
