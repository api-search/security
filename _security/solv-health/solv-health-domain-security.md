---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: solvhealth.com
  spf: true
hosts:
- cert_expires: Aug 11 22:46:59 2026 GMT
  host: www.solvhealth.com
  hsts: true
  hsts_max_age: 3153600000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solv Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solv Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Solv Health
provider_slug: solv-health
slug: solv-health-domain-security
source_filename: solv-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solvhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 22:46:59 2026 GMT\n  hsts: true\n  hsts_max_age: 3153600000\ndomains:\n- domain: solvhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solv-health/refs/heads/main/security/solv-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Urgent Care
- Appointment Booking
- EHR Interoperability
- HL7
- FHIR
- Digital Health
---
