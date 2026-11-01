---
api_specs:
- filename: microbilt-openapi-generated.yml
  format: yaml
  label: Microbilt API
  slug: microbilt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microbilt/openapi/_ae-authored/microbilt-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "DigiCert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microbilt.com
  spf: true
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: microbilt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Microbilt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microbilt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microbilt
provider_slug: microbilt
slug: microbilt-domain-security
source_filename: microbilt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: microbilt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microbilt.com\n  dnssec: false\n  caa:\n  - 0 issue \"DigiCert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microbilt/security/microbilt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Credit Decisioning
- Identity Verification
- Background Screening
- Business Credentialing
- Risk Management
- Alternative Credit Data
- Compliance
---
