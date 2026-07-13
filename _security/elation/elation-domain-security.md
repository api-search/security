---
api_specs:
- filename: llms.txt
  format: yaml
  label: Elation Health REST API
  slug: elation-health-api
  spec_type: OpenAPI
  url: https://docs.elationhealth.com/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elationhealth.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elationemr.com
  spf: true
hosts:
- cert_expires: Feb 20 23:59:59 2027 GMT
  host: www.elationhealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 08:56:34 2026 GMT
  host: docs.elationhealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: app.elationemr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elation Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Elation Health
provider_slug: elation
slug: elation-domain-security
source_filename: elation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.elationhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.elationhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:56:34 2026 GMT\n  hsts: null\n- host: app.elationemr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: elationhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: elationemr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elation/refs/heads/main/security/elation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- EHR
- Electronic Health Records
- Primary Care
- Healthcare
- FHIR
- Clinical
- Patients
- Prescriptions
- Messaging
---
