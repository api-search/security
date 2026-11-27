---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: evmux.com
  spf: true
hosts:
- cert_expires: Dec 11 13:38:35 2026 GMT
  host: evmux.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Evmux Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evmux, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Evmux
provider_slug: evmux-com
slug: evmux-com-domain-security
source_filename: evmux-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evmux.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 13:38:35 2026 GMT\n  hsts: false\ndomains:\n- domain: evmux.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/evmux-com/security/evmux-com-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Live Streaming
- Video
- Software-as-a-Service
- Media
- Production
---
