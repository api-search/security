---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: telus.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inputhealth.com
  spf: true
hosts:
- cert_expires: Sep 24 10:42:38 2026 GMT
  host: www.telus.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 00:34:14 2026 GMT
  host: help.inputhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: simplifier.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Telus Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TELUS Health, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TELUS Health
provider_slug: telus-health
slug: telus-health-domain-security
source_filename: telus-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.telus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:42:38 2026 GMT\n  hsts: null\n- host: help.inputhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 00:34:14 2026 GMT\n  hsts: false\n- host: simplifier.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: telus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: inputhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telus-health/refs/heads/main/security/telus-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Canada
- EMR
- EHR
- FHIR
- HL7
- Interoperability
- GraphQL
- e-Prescribing
- Pharmacy
- Digital Health
- Clinical Data
---
