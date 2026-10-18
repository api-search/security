---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bjstudios.be
  spf: true
hosts:
- cert_expires: Dec 19 21:10:30 2026 GMT
  host: www.bjstudios.be
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bjstudios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bjstudios, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bjstudios
provider_slug: bjstudios
slug: bjstudios-domain-security
source_filename: bjstudios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bjstudios.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 21:10:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: bjstudios.be\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bjstudios/refs/heads/main/security/bjstudios-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Event
- Live-Streaming
- LED-Wall
- Technology
- Belgium
---
