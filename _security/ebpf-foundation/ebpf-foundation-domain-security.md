---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ebpf.foundation
  spf: true
hosts:
- cert_expires: Aug 27 19:15:50 2026 GMT
  host: ebpf.foundation
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ebpf Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for eBPF Foundation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: eBPF Foundation
provider_slug: ebpf-foundation
slug: ebpf-foundation-domain-security
source_filename: ebpf-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ebpf.foundation\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: ebpf.foundation\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ebpf-foundation/refs/heads/main/security/ebpf-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- eBPF
- Kernel
- Linux Foundation
- Networking
- Observability
- Security
---
