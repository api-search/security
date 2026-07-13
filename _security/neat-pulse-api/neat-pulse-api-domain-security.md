---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: neat.no
  spf: true
hosts:
- cert_expires: Oct  3 09:44:28 2026 GMT
  host: pulse.neat.no
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neat Pulse Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neat Pulse API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Neat Pulse API
provider_slug: neat-pulse-api
slug: neat-pulse-api-domain-security
source_filename: neat-pulse-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pulse.neat.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:44:28 2026 GMT\n  hsts: null\ndomains:\n- domain: neat.no\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neat-pulse-api/refs/heads/main/security/neat-pulse-api-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Video Conferencing
- Devices
- Hardware
---
