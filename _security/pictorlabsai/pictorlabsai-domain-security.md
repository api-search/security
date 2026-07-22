---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pictorlabs.ai
  spf: true
hosts:
- cert_expires: Oct  5 20:43:11 2026 GMT
  host: www.pictorlabs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pictorlabsai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PictorLabs.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PictorLabs.ai
provider_slug: pictorlabsai
slug: pictorlabsai-domain-security
source_filename: pictorlabsai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pictorlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:43:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pictorlabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pictorlabsai/refs/heads/main/security/pictorlabsai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Digital Pathology
- Virtual Staining
- Histopathology
- Medical Imaging
- Healthcare
- Life Sciences
---
