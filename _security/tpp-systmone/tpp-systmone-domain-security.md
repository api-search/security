---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tpp-uk.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nhs.uk
  spf: true
hosts:
- cert_expires: Sep 19 23:09:55 2026 GMT
  host: tpp-uk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 21:58:44 2026 GMT
  host: digital.nhs.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tpp Systmone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TPP (SystmOne), probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TPP (SystmOne)
provider_slug: tpp-systmone
slug: tpp-systmone-domain-security
source_filename: tpp-systmone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tpp-uk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:09:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: digital.nhs.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 21:58:44 2026 GMT\n  hsts: null\ndomains:\n- domain: tpp-uk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: nhs.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tpp-systmone/refs/heads/main/security/tpp-systmone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- United Kingdom
- EHR
- EMR
- FHIR
- HL7
- Interoperability
- GP Connect
- IM1
- National Health System
- Primary Care
- Clinical System
---
