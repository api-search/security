---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: medthread.health
  spf: true
hosts:
- cert_expires: Aug 21 22:51:59 2026 GMT
  host: www.medthread.health
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Medthread Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MedThread, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MedThread
provider_slug: medthread
slug: medthread-domain-security
source_filename: medthread-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.medthread.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 22:51:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: medthread.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medthread/refs/heads/main/security/medthread-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Health Information Management
- Long-Term Care
- Post-Acute Care
- Skilled Nursing
- FHIR
- EHR Integration
- Compliance
- Patient Records
- Artificial Intelligence
---
