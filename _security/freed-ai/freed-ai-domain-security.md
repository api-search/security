---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getfreed.ai
  spf: true
hosts:
- cert_expires: Sep 14 10:14:48 2026 GMT
  host: www.getfreed.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freed Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freed, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Freed
provider_slug: freed-ai
slug: freed-ai-domain-security
source_filename: freed-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getfreed.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 10:14:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getfreed.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freed-ai/refs/heads/main/security/freed-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Scribe
- Medical Scribe
- Clinical Documentation
- Ambient Clinical Intelligence
- Healthcare AI
- SOAP Notes
- EHR Integration
- ICD-10 Coding
- CPT Coding
- HIPAA
- SOC 2
- Chrome Extension
- Clinician Productivity
- Consumer SaaS
---
