---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: relatable.io
  spf: false
hosts:
- cert_expires: Sep 15 12:00:31 2026 GMT
  host: relatable.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Relatableio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Relatable.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Relatable.io
provider_slug: relatableio
slug: relatableio-domain-security
source_filename: relatableio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: relatable.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 12:00:31 2026 GMT\n  hsts: false\ndomains:\n- domain: relatable.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relatableio/refs/heads/main/security/relatableio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- MedTech
- Medical Devices
- Healthcare
- Product Relationship Management
- Competitive Intelligence
- Data Integration
---
