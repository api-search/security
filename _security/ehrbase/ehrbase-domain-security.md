---
api_specs:
- filename: ehrbase-openehr-rest-api-openapi.json
  format: json
  label: EHRbase openEHR REST API
  slug: openehr-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ehrbase/refs/heads/main/openapi/ehrbase-openehr-rest-api-openapi.json
- filename: ehrbase-admin-api-openapi.json
  format: json
  label: EHRbase Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ehrbase/refs/heads/main/openapi/ehrbase-admin-api-openapi.json
- filename: ehrbase-status-api-openapi.json
  format: json
  label: EHRbase Status and Metrics API
  slug: status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ehrbase/refs/heads/main/openapi/ehrbase-status-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ehrbase.org
  spf: false
hosts:
- cert_expires: Oct 22 23:16:14 2026 GMT
  host: ehrbase.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 03:15:58 2026 GMT
  host: sandkiste.ehrbase.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ehrbase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EHRbase, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: EHRbase
provider_slug: ehrbase
slug: ehrbase-domain-security
source_filename: ehrbase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ehrbase.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:16:14 2026 GMT\n  hsts: false\n- host: sandkiste.ehrbase.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 03:15:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ehrbase.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ehrbase/refs/heads/main/security/ehrbase-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Health IT
- Electronic Health Records
- Clinical Data
- openEHR
- Interoperability
- Open Source
- Databases
- Standards
---
