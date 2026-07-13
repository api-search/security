---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloudwego.io
  spf: true
hosts:
- cert_expires: Sep 20 16:18:22 2026 GMT
  host: www.cloudwego.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kitex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kitex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kitex
provider_slug: kitex
slug: kitex-domain-security
source_filename: kitex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudwego.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 16:18:22 2026 GMT\n  hsts: false\ndomains:\n- domain: cloudwego.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kitex/refs/heads/main/security/kitex-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Frameworks
- Go
- High Performance
- Microservices
- Protocol Buffers
- RPC
- Thrift
---
