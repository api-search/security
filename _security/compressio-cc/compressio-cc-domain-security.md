---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: compressio.cc
  spf: false
hosts:
- cert_expires: Dec 15 17:14:07 2026 GMT
  host: compressio.cc
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 14:21:22 2027 GMT
  host: api.compressio.cc
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: CompressIO Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CompressIO, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CompressIO
provider_slug: compressio-cc
slug: compressio-cc-domain-security
source_filename: compressio-cc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compressio.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 17:14:07 2026 GMT\n  hsts: false\n- host: api.compressio.cc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 14:21:22 2027 GMT\n  hsts: null\ndomains:\n- domain: compressio.cc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/compressio-cc/security/compressio-cc-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Image Compression
- Image Conversion
- Image Processing
- MCP
- AI Agents
- WebAssembly
---
