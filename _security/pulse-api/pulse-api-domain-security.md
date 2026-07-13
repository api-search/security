---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pulsepro.ai
  spf: false
hosts:
- cert_expires: Oct  8 09:06:03 2026 GMT
  host: docs.pulsepro.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pulse Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pulse API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Pulse API
provider_slug: pulse-api
slug: pulse-api-domain-security
source_filename: pulse-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.pulsepro.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 09:06:03 2026 GMT\n  hsts: null\ndomains:\n- domain: pulsepro.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulse-api/refs/heads/main/security/pulse-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Pulse
- Account
- Data
---
