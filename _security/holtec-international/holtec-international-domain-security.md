---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: holtecinternational.com
  spf: true
hosts:
- cert_expires: Aug 18 17:37:19 2026 GMT
  host: holtecinternational.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Holtec International Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Holtec International, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Holtec International
provider_slug: holtec-international
slug: holtec-international-domain-security
source_filename: holtec-international-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: holtecinternational.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 17:37:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: holtecinternational.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holtec-international/refs/heads/main/security/holtec-international-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Clean Energy
- Decommissioning
- Energy
- Nuclear
- Nuclear Fuel
- Palisades
- Reactor
- SMR-300
- Small Modular Reactor
- Spent Fuel Storage
---
