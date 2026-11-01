---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: token-counter.app
  spf: false
hosts:
- cert_expires: Jan 13 21:22:16 2027 GMT
  host: token-counter.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Token Counter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LLM Token Counter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LLM Token Counter
provider_slug: token-counter
slug: token-counter-domain-security
source_filename: token-counter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: token-counter.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 21:22:16 2027 GMT\n  hsts: false\ndomains:\n- domain: token-counter.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/token-counter/security/token-counter-domain-security.yml
summary_line: TLSv1.3
tags:
- LLM pricing
- Token counting
- API cost calculator
---
