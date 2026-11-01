---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: imvision.ai
  spf: true
hosts:
- cert_expires: Dec  6 11:06:35 2026 GMT
  host: imvision.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Imvision Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for imvision, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: imvision
provider_slug: imvision
slug: imvision-domain-security
source_filename: imvision-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: imvision.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 11:06:35 2026 GMT\n  hsts: null\ndomains:\n- domain: imvision.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/imvision/security/imvision-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Computer Vision
- Manufacturing
- Quality Control
- Automation
---
