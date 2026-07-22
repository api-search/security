---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ambiencehealthcare.com
  spf: true
hosts:
- cert_expires: Aug 22 21:49:39 2026 GMT
  host: www.ambiencehealthcare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ambience Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ambience Healthcare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ambience Healthcare
provider_slug: ambience-ai
slug: ambience-ai-domain-security
source_filename: ambience-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ambiencehealthcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 21:49:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ambiencehealthcare.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambience-ai/refs/heads/main/security/ambience-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- Clinical AI
- Ambient AI
- AI Medical Scribe
- Clinical Documentation
- Medical Coding
- Revenue Cycle
- HCC
- ICD-10
- CPT
- Electronic Health Record
- EHR Integration
- Epic
- Cerner
- Athenahealth
- FHIR
- SMART on FHIR
- HIPAA
- Hospitals
- Health Systems
- Generative AI
---
