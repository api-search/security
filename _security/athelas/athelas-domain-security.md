---
api_specs:
- filename: athelas-enterprise-openapi.yml
  format: yaml
  label: Athelas Enterprise API
  slug: athelas-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/athelas/refs/heads/main/openapi/athelas-enterprise-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: Quarantine
  dnssec: false
  domain: athelas.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Oct  3 06:32:14 2026 GMT
  host: athelas.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: athelas.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 11:56:21 2026 GMT
  host: api.athelas.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Athelas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Athelas, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=Quarantine).'
provider_name: Athelas
provider_slug: athelas
slug: athelas-domain-security
source_filename: athelas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: athelas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:32:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: athelas.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.athelas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 11:56:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: athelas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: Quarantine\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/athelas/refs/heads/main/security/athelas-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Remote Patient Monitoring
- Electronic Health Records
- FHIR
- Revenue Cycle Management
- Medical Devices
- SMART on FHIR
- Interoperability
- AI
---
