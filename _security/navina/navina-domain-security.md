---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: navina.ai
  spf: true
hosts:
- cert_expires: Oct  3 06:29:10 2026 GMT
  host: www.navina.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Navina Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Navina, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Navina
provider_slug: navina
slug: navina-domain-security
source_filename: navina-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.navina.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:29:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: navina.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navina/refs/heads/main/security/navina-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Artificial Intelligence
- Clinical Decision Support
- Value-Based Care
- Risk Adjustment
- Electronic Health Records
- FHIR
- Interoperability
- Medical Coding
---
