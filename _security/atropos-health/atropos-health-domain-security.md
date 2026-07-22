---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: atroposhealth.com
  spf: true
hosts:
- cert_expires: Sep 29 18:54:11 2026 GMT
  host: www.atroposhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Atropos Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atropos Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Atropos Health
provider_slug: atropos-health
slug: atropos-health-domain-security
source_filename: atropos-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atroposhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:54:11 2026 GMT\n  hsts: false\ndomains:\n- domain: atroposhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atropos-health/refs/heads/main/security/atropos-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real World Evidence
- Real World Data
- Clinical Evidence
- Observational Studies
- Healthcare Analytics
- Health Data
- Generative AI
- Agentic AI
- Clinical Decision Support
- Life Sciences
- Health Systems
- Pharma
- HEOR
- Federated Analytics
- Temporal Query Language
- Patient Timelines
- GENEVA OS
- ChatRWD
- Alexandria
- Green Button
- Stanford Spinout
---
