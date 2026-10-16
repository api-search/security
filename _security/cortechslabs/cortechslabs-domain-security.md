---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cortechs.ai
  spf: true
hosts:
- cert_expires: Nov 22 06:43:25 2026 GMT
  host: www.cortechs.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cortechslabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cortechslabs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cortechslabs
provider_slug: cortechslabs
slug: cortechslabs-domain-security
source_filename: cortechslabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cortechs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 06:43:25 2026 GMT\n  hsts: false\ndomains:\n- domain: cortechs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cortechslabs/refs/heads/main/security/cortechslabs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Medical Imaging
- Brain Segmentation
- Healthcare
---
