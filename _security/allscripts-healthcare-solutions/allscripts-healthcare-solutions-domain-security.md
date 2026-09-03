---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: allscripts.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: veradigm.com
  spf: true
hosts:
- cert_expires: Feb 21 23:59:59 2027 GMT
  host: www.allscripts.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 08:19:08 2027 GMT
  host: developer.veradigm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 21 17:35:31 2027 GMT
  host: fhir.fhirpoint.open.allscripts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Allscripts Healthcare Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allscripts Healthcare Solutions, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Allscripts Healthcare Solutions
provider_slug: allscripts-healthcare-solutions
slug: allscripts-healthcare-solutions-domain-security
source_filename: allscripts-healthcare-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.allscripts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.veradigm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 13 08:19:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fhir.fhirpoint.open.allscripts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 17:35:31 2027 GMT\n  hsts: null\ndomains:\n- domain: allscripts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: veradigm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allscripts-healthcare-solutions/refs/heads/main/security/allscripts-healthcare-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare IT
- EHR
- Clinical
- FHIR
- HL7
- SMART on FHIR
- USCDI
- Interoperability
- Patient Access
- 21st Century Cures
- Veradigm
---
