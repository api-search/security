---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: terrafirma.inc
  spf: true
hosts:
- cert_expires: Sep 20 19:29:14 2026 GMT
  host: terrafirma.inc
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Terrafirma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TerraFirma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TerraFirma
provider_slug: terrafirma
slug: terrafirma-domain-security
source_filename: terrafirma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: terrafirma.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 19:29:14 2026 GMT\n  hsts: false\ndomains:\n- domain: terrafirma.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terrafirma/refs/heads/main/security/terrafirma-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Physical Ai
- Robotics
- Construction
- Autonomous Systems
- Construction Technology
- Heavy Equipment
---
