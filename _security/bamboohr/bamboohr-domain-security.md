---
api_specs:
- filename: bamboohr-openapi.yml
  format: yaml
  label: BambooHR REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bamboohr/refs/heads/main/openapi/bamboohr-openapi.yml
- filename: bamboohr-asyncapi.yml
  format: yaml
  label: BambooHR Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bamboohr/refs/heads/main/openapi/bamboohr-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bamboohr.com
  spf: true
hosts:
- cert_expires: Sep 12 01:43:57 2026 GMT
  host: www.bamboohr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 02:39:04 2026 GMT
  host: documentation.bamboohr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 18:32:46 2026 GMT
  host: api.bamboohr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bamboohr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BambooHR, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BambooHR
provider_slug: bamboohr
slug: bamboohr-domain-security
source_filename: bamboohr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bamboohr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 01:43:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: documentation.bamboohr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:39:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bamboohr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 18:32:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bamboohr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bamboohr/refs/heads/main/security/bamboohr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- HRIS
- Human Resources
- Payroll
- Time Tracking
- Applicant Tracking
- Performance Management
---
