---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ebpf.io
  spf: false
hosts:
- cert_expires: Oct  6 00:21:45 2026 GMT
  host: ebpf.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ebpf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eBPF, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: eBPF
provider_slug: ebpf
slug: ebpf-domain-security
source_filename: ebpf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ebpf.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:21:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ebpf.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ebpf/refs/heads/main/security/ebpf-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- eBPF
- Kernel
- Linux
- Networking
- Observability
- Security
- Tracing
---
