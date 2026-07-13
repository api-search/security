---
api_specs:
- filename: humana-openapi.yml
  format: yaml
  label: Humana FHIR Clinical Data API
  slug: humana-fhir-clinical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humana/refs/heads/main/openapi/humana-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: humana.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: developers.humana.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: www.humana.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: fhir.humana.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Humana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humana, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Humana
provider_slug: humana
slug: humana-domain-security
source_filename: humana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.humana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.humana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fhir.humana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: humana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humana/refs/heads/main/security/humana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- FHIR
- Health Insurance
- Healthcare
- Interoperability
- Medicare
- Fortune 100
---
