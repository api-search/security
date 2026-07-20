---
api_specs:
- filename: clover-health-fhir-openapi-original.yml
  format: yaml
  label: Clover Health FHIR API (Formulary & Provider Directory)
  slug: clover-health-fhir-api-formulary-provider-directory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clover-health/refs/heads/main/openapi/clover-health-fhir-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloverhealth.com
  spf: true
hosts:
- cert_expires: Sep  5 11:54:15 2026 GMT
  host: www.cloverhealth.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- host: public-api.cloverhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clover Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clover Health, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clover Health
provider_slug: clover-health
slug: clover-health-domain-security
source_filename: clover-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloverhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 11:54:15 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: public-api.cloverhealth.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: false\ndomains:\n- domain: cloverhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clover-health/refs/heads/main/security/clover-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Health Insurance
- Medicare Advantage
- FHIR
- Interoperability
- Provider Directory
- Formulary
- Patient Access
- Payer
---
