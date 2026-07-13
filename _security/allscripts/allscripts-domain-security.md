---
api_specs:
- filename: Considerations.html
  format: yaml
  label: Veradigm FHIR R4 API
  slug: veradigm-fhir-r4-api
  spec_type: OpenAPI
  url: https://developer.veradigm.com/Content/fhir/GetStarted/Concepts/Considerations.html
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: veradigm.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: allscripts.com
  spf: true
hosts:
- cert_expires: Sep  3 12:50:11 2026 GMT
  host: developer.veradigm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jul 21 17:05:14 2026 GMT
  host: open.platform.veradigm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.allscripts.com
  https: false
kind: domain-security
layout: security
method: probed
name: Allscripts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Allscripts, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Allscripts
provider_slug: allscripts
slug: allscripts-domain-security
source_filename: allscripts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.veradigm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  3 12:50:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: open.platform.veradigm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 21 17:05:14 2026 GMT\n  hsts: null\n- host: developer.allscripts.com\n  https: false\ndomains:\n- domain: veradigm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: allscripts.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allscripts/refs/heads/main/security/allscripts-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Healthcare IT
- EHR
- FHIR
- Clinical Data
- Practice Management
- HL7
---
