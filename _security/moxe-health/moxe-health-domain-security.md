---
api_specs:
- filename: moxe-health-chart-retrieval-initiate-openapi.json
  format: json
  label: Moxe Health Chart Retrieval API
  slug: moxe-health-chart-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moxe-health/refs/heads/main/openapi/moxe-health-chart-retrieval-initiate-openapi.json
- filename: moxe-health-claim-management-initiate-openapi.json
  format: json
  label: Moxe Health Claim Management API
  slug: moxe-health-claim-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moxe-health/refs/heads/main/openapi/moxe-health-claim-management-initiate-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moxehealth.com
  spf: true
hosts:
- cert_expires: Sep 28 06:14:36 2026 GMT
  host: moxehealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 09:34:42 2026 GMT
  host: developer.moxehealth.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: int-api.moxehealth.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moxe Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moxe Health, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Moxe Health
provider_slug: moxe-health
slug: moxe-health-domain-security
source_filename: moxe-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moxehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 06:14:36 2026 GMT\n  hsts: false\n- host: developer.moxehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 09:34:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: int-api.moxehealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: moxehealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moxe-health/refs/heads/main/security/moxe-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- United States
- Interoperability
- Clinical Data
- Payer
- Provider
- EHR
- Health Data Exchange
- Claims
- Risk Adjustment
---
