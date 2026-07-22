---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: camfer.dev
  spf: false
hosts:
- cert_expires: Aug 29 04:50:14 2026 GMT
  host: camfer.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Camfer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Camfer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Camfer
provider_slug: camfer
slug: camfer-domain-security
source_filename: camfer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: camfer.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 04:50:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: camfer.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/camfer/refs/heads/main/security/camfer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Computer-Aided Design
- CAD
- Mechanical Engineering
- Artificial Intelligence
- Generative Design
- SolidWorks
- Text-to-CAD
- Desktop Application
---
