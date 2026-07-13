---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bytecodealliance.org
  spf: false
- caa: []
  dmarc: false
  dnssec: true
  domain: wasi.dev
  spf: false
hosts:
- cert_expires: Sep 29 05:35:19 2026 GMT
  host: component-model.bytecodealliance.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 19:28:23 2026 GMT
  host: wasi.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 14:16:23 2026 GMT
  host: bytecodealliance.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Component Model Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Component Model, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Component Model
provider_slug: component-model
slug: component-model-domain-security
source_filename: component-model-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: component-model.bytecodealliance.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:35:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: wasi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 19:28:23 2026 GMT\n  hsts: false\n- host: bytecodealliance.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:16:23 2026 GMT\n  hsts: false\ndomains:\n- domain: bytecodealliance.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: wasi.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/component-model/refs/heads/main/security/component-model-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- ABI
- Bytecode Alliance
- Component
- Interface
- Modular
- Specification
- WASI
- WebAssembly
- WIT
- World
---
