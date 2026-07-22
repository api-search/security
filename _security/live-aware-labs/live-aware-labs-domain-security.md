---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: liveaware.io
  spf: false
hosts:
- cert_expires: Oct  1 17:27:32 2026 GMT
  host: www.liveaware.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Live Aware Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Live Aware Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Live Aware Labs
provider_slug: live-aware-labs
slug: live-aware-labs-domain-security
source_filename: live-aware-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liveaware.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 17:27:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: liveaware.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/live-aware-labs/refs/heads/main/security/live-aware-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Game Development
- Playtesting
- Player Analytics
- Game Analytics
- Video Telemetry
- Developer Tools
- Artificial Intelligence
---
