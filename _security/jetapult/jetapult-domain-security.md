---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jetapult.co
  spf: false
hosts:
- cert_expires: Oct 13 13:24:38 2026 GMT
  host: www.jetapult.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jetapult Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jetapult, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Jetapult
provider_slug: jetapult
slug: jetapult-domain-security
source_filename: jetapult-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jetapult.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 13:24:38 2026 GMT\n  hsts: false\ndomains:\n- domain: jetapult.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetapult/refs/heads/main/security/jetapult-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Consumer
- Gaming
- Mobile Games
- Game Studios
- Monetization
- Artificial Intelligence
- Venture Capital
---
