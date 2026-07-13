---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Fasten Connect API
  slug: fasten-connect
  spec_type: OpenAPI
  url: https://docs.connect.fastenhealth.com/api-reference/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fastenhealth.com
  spf: true
hosts:
- cert_expires: Sep  5 03:54:51 2026 GMT
  host: www.fastenhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 02:38:24 2026 GMT
  host: docs.connect.fastenhealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: api.connect.fastenhealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fasten Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fasten Health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fasten Health
provider_slug: fasten-health
slug: fasten-health-domain-security
source_filename: fasten-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fastenhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 03:54:51 2026 GMT\n  hsts: false\n- host: docs.connect.fastenhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:38:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.connect.fastenhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: fastenhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fasten-health/refs/heads/main/security/fasten-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- FHIR
- Personal Health Record
- Electronic Medical Record
- Health Data Interoperability
- TEFCA
- EHI Export
- Patient Consent
- Self-Hosted
- Open Source
- HL7
- Healthcare Connectivity
---
