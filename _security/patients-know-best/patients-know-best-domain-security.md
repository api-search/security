---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: patientsknowbest.com
  spf: true
hosts:
- cert_expires: Sep 15 16:40:29 2026 GMT
  host: patientsknowbest.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 06:13:00 2026 GMT
  host: wiki.patientsknowbest.com
  hsts: true
  hsts_max_age: 34560000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 12:24:17 2026 GMT
  host: my.patientsknowbest.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Patients Know Best Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Patients Know Best, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Patients Know Best
provider_slug: patients-know-best
slug: patients-know-best-domain-security
source_filename: patients-know-best-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: patientsknowbest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:40:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wiki.patientsknowbest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:13:00 2026 GMT\n  hsts: true\n  hsts_max_age: 34560000\n- host: my.patientsknowbest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 12:24:17 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: patientsknowbest.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patients-know-best/refs/heads/main/security/patients-know-best-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Healthcare
- Electronic Health Records
- Personal Health Record
- FHIR
- Interoperability
- NHS
- Patient Data
- Medical Records
---
