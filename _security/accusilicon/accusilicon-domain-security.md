---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: accusilicon.com
  spf: true
hosts:
- cert_expires: Dec  3 18:16:45 2026 GMT
  host: accusilicon.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Accusilicon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Accusilicon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Accusilicon
provider_slug: accusilicon
slug: accusilicon-domain-security
source_filename: accusilicon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: accusilicon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 18:16:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: accusilicon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accusilicon/refs/heads/main/security/accusilicon-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Semiconductors
- Integrated Circuits
- Clock Chips
- Oscillators
- Timing
- Audio
- Hardware
- Electronics
---
