---
api_specs:
- filename: santevet-toolkit-openapi.yml
  format: yaml
  label: SantéVet Toolkit API
  slug: santevet-toolkit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santevet/refs/heads/main/openapi/santevet-toolkit-openapi.yml
- filename: santevet-reimbursement-openapi.yml
  format: yaml
  label: SantéVet Reimbursement API
  slug: santevet-reimbursement
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/santevet/refs/heads/main/openapi/santevet-reimbursement-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: santevet.com
  spf: true
hosts:
- cert_expires: Nov  7 18:37:57 2026 GMT
  host: www.santevet.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: reimbursement.api.santevet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: staging.reimbursement.api.santevet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Santevet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SantéVet, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SantéVet
provider_slug: santevet
slug: santevet-domain-security
source_filename: santevet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.santevet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 18:37:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: reimbursement.api.santevet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: null\n- host: staging.reimbursement.api.santevet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: santevet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/santevet/refs/heads/main/security/santevet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Insurtech
- Pet Insurance
- Veterinary
- Consumer
- Embedded Insurance
- Claims
- Payments
- France
- Europe
- Company
---
