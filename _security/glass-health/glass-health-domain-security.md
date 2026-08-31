---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: glass.health
  spf: true
hosts:
- cert_expires: Sep 17 05:06:10 2026 GMT
  host: glass.health
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Glass Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Glass Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Glass Health
provider_slug: glass-health
slug: glass-health-domain-security
source_filename: glass-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: glass.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 05:06:10 2026 GMT\n  hsts: false\ndomains:\n- domain: glass.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/glass-health/refs/heads/main/security/glass-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Clinical Decision Support
- Diagnostic AI
- Differential Diagnosis
- Ambient Scribing
- Clinical Documentation
- Medical AI
- Generative AI
- EHR Integration
- SMART On FHIR
- Evidence Based Medicine
- Physician Copilot
---
