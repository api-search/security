---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: simantic.dev
  spf: true
hosts:
- cert_expires: Sep 14 13:20:58 2026 GMT
  host: simantic.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simantic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simantic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Simantic
provider_slug: simantic
slug: simantic-domain-security
source_filename: simantic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simantic.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:20:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: simantic.dev\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simantic/refs/heads/main/security/simantic-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Firmware
- Embedded Systems
- Hardware Simulation
- Developer Tools
- Testing
- Quality Assurance
- Microcontroller
- AI Agents
- Model Context Protocol
- Semiconductors
- Continuous Integration
---
