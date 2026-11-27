---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chamade.io
  spf: false
hosts:
- cert_expires: Jan 27 11:26:45 2027 GMT
  host: chamade.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chamade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chamade, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Chamade
provider_slug: chamade-io
slug: chamade-io-domain-security
source_filename: chamade-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chamade.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 11:26:45 2027 GMT\n  hsts: null\ndomains:\n- domain: chamade.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/chamade-io/security/chamade-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Voice gateway
- Chat gateway
- AI Agents
- SIP
- Speech API
---
