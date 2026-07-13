---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: protobuf.dev
  spf: true
hosts:
- cert_expires: Sep 19 19:13:20 2026 GMT
  host: protobuf.dev
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Protocol Buffers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Protocol Buffers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Protocol Buffers
provider_slug: protocol-buffers
slug: protocol-buffers-domain-security
source_filename: protocol-buffers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: protobuf.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:13:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: protobuf.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/protocol-buffers/refs/heads/main/security/protocol-buffers-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Format
- gRPC
- Protobuf
- Protocol Buffers
- Serialization
---
