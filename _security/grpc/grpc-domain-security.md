---
api_specs:
- filename: openapi.yml
  format: yaml
  label: gRPC-Web Proxy API
  slug: grpc-web-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grpc/refs/heads/main/openapi.yml
- filename: asyncapi.yml
  format: yaml
  label: gRPC Health Checking Service
  slug: grpc-health-checking
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/grpc/refs/heads/main/asyncapi.yml
- filename: asyncapi.yml
  format: yaml
  label: gRPC Server Reflection
  slug: grpc-server-reflection
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/grpc/refs/heads/main/asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: grpc.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: protobuf.dev
  spf: true
hosts:
- cert_expires: Sep 10 10:25:02 2026 GMT
  host: grpc.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 19:13:20 2026 GMT
  host: protobuf.dev
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grpc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for gRPC, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: gRPC
provider_slug: grpc
slug: grpc-domain-security
source_filename: grpc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grpc.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 10:25:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: protobuf.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 19:13:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: grpc.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: protobuf.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grpc/refs/heads/main/security/grpc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CNCF
- HTTP/2
- Microservices
- Protocol Buffers
- RPC
---
