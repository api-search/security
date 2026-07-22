---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: scripted.co
  spf: false
hosts:
- cert_expires: Oct  3 00:35:45 2026 GMT
  host: scripted.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Script Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Script Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Script Health
provider_slug: script-health
slug: script-health-domain-security
source_filename: script-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scripted.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:35:45 2026 GMT\n  hsts: false\ndomains:\n- domain: scripted.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/script-health/refs/heads/main/security/script-health-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Pharmacy
- Telehealth
- Prescriptions
- Clinical Services
- Health
- Medical Billing
---
