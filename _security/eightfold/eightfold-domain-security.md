---
api_specs:
- filename: llms.txt
  format: yaml
  label: Eightfold API v2
  slug: eightfold-api-v2
  spec_type: OpenAPI
  url: https://apidocs.eightfold.ai/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eightfold.ai
  spf: true
hosts:
- cert_expires: Sep 17 19:59:24 2026 GMT
  host: eightfold.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 12:57:17 2026 GMT
  host: apidocs.eightfold.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: apiv2.eightfold.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eightfold Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eightfold, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eightfold
provider_slug: eightfold
slug: eightfold-domain-security
source_filename: eightfold-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eightfold.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:59:24 2026 GMT\n  hsts: false\n- host: apidocs.eightfold.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 12:57:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apiv2.eightfold.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: eightfold.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eightfold/refs/heads/main/security/eightfold-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Talent Intelligence
- Talent Acquisition
- Talent Management
- Recruiting
- Human Resources
- Workforce Planning
- HRIS
- ATS
- Artificial Intelligence
- SCIM
- REST
---
