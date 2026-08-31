---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lightelligence.ai
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: www.lightelligence.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lightelligence
provider_slug: lightelligence
slug: lightelligence-domain-security
source_filename: lightelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lightelligence.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: lightelligence.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightelligence/refs/heads/main/security/lightelligence-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Optical Computing
- Photonics
- Semiconductors
- AI Infrastructure
- Hardware Accelerators
- High Performance Computing
- Optical Interconnect
- Data-Center
---
