---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lumilens.com
  spf: true
hosts:
- cert_expires: Nov 22 07:30:51 2026 GMT
  host: lumilens.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lumilens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumilens, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lumilens
provider_slug: lumilens
slug: lumilens-domain-security
source_filename: lumilens-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lumilens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 07:30:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lumilens.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumilens/refs/heads/main/security/lumilens-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Photonics
- Optical Networking
- Interconnects
- Semiconductors
- Silicon Photonics
- Data Centers
- Artificial Intelligence
- Hardware
---
