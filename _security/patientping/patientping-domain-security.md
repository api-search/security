---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: patientping.com
  spf: true
hosts:
- cert_expires: Sep 13 18:54:05 2026 GMT
  host: patientping.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Patientping Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PatientPing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PatientPing
provider_slug: patientping
slug: patientping-domain-security
source_filename: patientping-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: patientping.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:54:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: patientping.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patientping/refs/heads/main/security/patientping-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Bio Healthcare
- Care Coordination
- Health IT
- Interoperability
- Notifications
- HL7 ADT
---
