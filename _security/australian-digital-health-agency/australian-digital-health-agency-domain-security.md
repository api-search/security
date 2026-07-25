---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: digitalhealth.gov.au
  spf: true
hosts:
- cert_expires: Oct  4 00:55:37 2026 GMT
  host: www.digitalhealth.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 00:55:37 2026 GMT
  host: implementer.digitalhealth.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 21:48:59 2026 GMT
  host: developer.digitalhealth.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Australian Digital Health Agency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Australian Digital Health Agency, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Australian Digital Health Agency
provider_slug: australian-digital-health-agency
slug: australian-digital-health-agency-domain-security
source_filename: australian-digital-health-agency-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digitalhealth.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 00:55:37 2026 GMT\n  hsts: null\n- host: implementer.digitalhealth.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 00:55:37 2026 GMT\n  hsts: null\n- host: developer.digitalhealth.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:48:59 2026 GMT\n  hsts: null\ndomains:\n- domain: digitalhealth.gov.au\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/australian-digital-health-agency/refs/heads/main/security/australian-digital-health-agency-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Healthcare
- Australia
- National Health System
- FHIR
- HL7
- Interoperability
- SMART on FHIR
- Electronic Health Record
- e-Prescribing
- Terminology
- Government
---
