---
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: riscv.org
  spf: true
hosts:
- cert_expires: Aug 26 11:33:14 2026 GMT
  host: riscv.org
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Risc V Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RISC-V International, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: RISC-V International
provider_slug: risc-v
slug: risc-v-domain-security
source_filename: risc-v-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: riscv.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 11:33:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: riscv.org\n  dnssec: false\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/risc-v/refs/heads/main/security/risc-v-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- C API
- Compiler
- Hardware
- Instruction Set Architecture
- Linux Foundation
- Open Hardware
- Open Source
- Processor
- RISC-V
- Simulator
---
