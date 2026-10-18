---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: circuitandchisel.com
  spf: false
hosts:
- cert_expires: Dec  7 13:51:42 2026 GMT
  host: circuitandchisel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Circuit Chisel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Circuit & Chisel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Circuit & Chisel
provider_slug: circuit-chisel
slug: circuit-chisel-domain-security
source_filename: circuit-chisel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: circuitandchisel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 13:51:42 2026 GMT\n  hsts: false\ndomains:\n- domain: circuitandchisel.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circuit-chisel/refs/heads/main/security/circuit-chisel-domain-security.yml
summary_line: TLSv1.3
tags:
- AI Platform
- CLI
- Frontier AI
- Token Pricing
---
