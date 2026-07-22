---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trackonomy.ai
  spf: false
hosts:
- cert_expires: Sep  4 03:04:28 2026 GMT
  host: trackonomy.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trackonomy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trackonomy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Trackonomy
provider_slug: trackonomy
slug: trackonomy-domain-security
source_filename: trackonomy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trackonomy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 03:04:28 2026 GMT\n  hsts: false\ndomains:\n- domain: trackonomy.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trackonomy/refs/heads/main/security/trackonomy-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Internet of Things
- Supply Chain
- Logistics
- Asset Tracking
- Smart Labels
- Sensors
---
