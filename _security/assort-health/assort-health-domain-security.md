---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: assorthealth.com
  spf: true
hosts:
- cert_expires: Sep 10 04:42:55 2026 GMT
  host: assorthealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Assort Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Assort Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Assort Health
provider_slug: assort-health
slug: assort-health-domain-security
source_filename: assort-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: assorthealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 04:42:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: assorthealth.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assort-health/refs/heads/main/security/assort-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Healthcare AI
- AI Voice Agents
- Conversational AI
- Patient Access
- Appointment Scheduling
- Patient Intake
- EHR Integration
- Revenue Cycle
---
