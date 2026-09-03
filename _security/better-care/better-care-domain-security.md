---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: better.care
  spf: true
hosts:
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: www.better.care
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: docs.better.care
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Better Care Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Better, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Better
provider_slug: better-care
slug: better-care-domain-security
source_filename: better-care-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.better.care\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: false\n- host: docs.better.care\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: better.care\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/better-care/refs/heads/main/security/better-care-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Healthcare
- openEHR
- Electronic Health Records
- Clinical Data
- Interoperability
- HL7 FHIR
- Medication Management
- Digital Health
- Low Code
- AQL
- Slovenia
---
