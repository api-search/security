---
api_specs:
- filename: penn-medicine-fhir-r4-openapi.yml
  format: yaml
  label: Penn Medicine FHIR R4 API
  slug: penn-medicine-fhir-r4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/penn-medicine/refs/heads/main/openapi/penn-medicine-fhir-r4-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pennmedicine.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: pennhealth.com
  spf: false
hosts:
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: www.pennmedicine.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: ssproxy.pennhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: secure.mypennmedicine.org
  hsts: true
  hsts_max_age: 16070400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Penn Medicine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Penn Medicine, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Penn Medicine
provider_slug: penn-medicine
slug: penn-medicine-domain-security
source_filename: penn-medicine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pennmedicine.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ssproxy.pennhealth.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: false\n- host: secure.mypennmedicine.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 16070400\ndomains:\n- domain: pennmedicine.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pennhealth.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/penn-medicine/refs/heads/main/security/penn-medicine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Hospital
- Academic Medical Center
- FHIR
- SMART On FHIR
- Patient Access
- Provider Directory
- CMS Interoperability
- US Core
- Bulk Data
- Epic
---
