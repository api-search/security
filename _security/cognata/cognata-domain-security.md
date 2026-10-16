---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cognata.com
  spf: true
hosts:
- cert_expires: Nov 27 22:21:15 2026 GMT
  host: www.cognata.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cognata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cognata
provider_slug: cognata
slug: cognata-domain-security
source_filename: cognata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cognata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 22:21:15 2026 GMT\n  hsts: false\ndomains:\n- domain: cognata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognata/refs/heads/main/security/cognata-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Autonomous Vehicles
- Simulation
- Defense
- Off‑Road
- Hardware Retrofit
- AI Data Augmentation
- Sensor Fusion
---
