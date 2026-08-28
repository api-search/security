---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sionpower.com
  spf: true
hosts:
- cert_expires: Nov  1 20:30:41 2026 GMT
  host: sionpower.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sion Power Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sion Power, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sion Power
provider_slug: sion-power
slug: sion-power-domain-security
source_filename: sion-power-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sionpower.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 20:30:41 2026 GMT\n  hsts: false\ndomains:\n- domain: sionpower.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sion-power/refs/heads/main/security/sion-power-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Batteries
- Energy Storage
- Lithium Metal
- Manufacturing
- Advanced Materials
- Defense
- Aerospace
- Electric Vehicles
- Hardware
---
