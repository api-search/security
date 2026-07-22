---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: helloeos.ai
  spf: true
hosts:
- cert_expires: Sep 30 13:55:16 2026 GMT
  host: www.helloeos.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eos Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eos AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Eos AI
provider_slug: eos-ai
slug: eos-ai-domain-security
source_filename: eos-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.helloeos.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 13:55:16 2026 GMT\n  hsts: false\ndomains:\n- domain: helloeos.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eos-ai/refs/heads/main/security/eos-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Healthcare
- AI
- Machine Learning
- Clinical Data
- Data Harmonization
- Medical Imaging
- Predictive Analytics
- Hospital Operations
---
