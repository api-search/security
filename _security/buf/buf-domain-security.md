---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: buf.build
  spf: false
hosts:
- cert_expires: Sep 19 00:46:30 2026 GMT
  host: buf.build
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Buf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Buf
provider_slug: buf
slug: buf-domain-security
source_filename: buf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buf.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 00:46:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: buf.build\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buf/refs/heads/main/security/buf-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Code Generation
- gRPC
- Kafka
- Open Source
- Protocol Buffers
- Schema Registry
- SDKs
- Streaming
---
