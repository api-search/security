---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: goreplay.org
  spf: false
hosts:
- cert_expires: Oct 28 17:07:50 2026 GMT
  host: goreplay.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Goreplay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoReplay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: GoReplay
provider_slug: goreplay
slug: goreplay-domain-security
source_filename: goreplay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goreplay.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 17:07:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: goreplay.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goreplay/refs/heads/main/security/goreplay-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API Testing
- HTTP Traffic
- Load Testing
- Network Capture
- Open-Source
- Traffic Replay
---
