---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: narrivela.com
  spf: false
hosts:
- cert_expires: Jan 11 07:18:29 2027 GMT
  host: narrivela.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Narrivela Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Narrivela, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Narrivela
provider_slug: narrivela-com
slug: narrivela-com-domain-security
source_filename: narrivela-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: narrivela.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 07:18:29 2027 GMT\n  hsts: false\ndomains:\n- domain: narrivela.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/narrivela-com/security/narrivela-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Voiceover
- Artificial Intelligence
- Speech
- MCP
- Audio
---
