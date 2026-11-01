---
api_specs:
- filename: qi-tech-openapi-generated.yml
  format: yaml
  label: QI Tech API
  slug: qi-tech-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qi-tech/openapi/_ae-authored/qi-tech-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: qitech.com.br
  spf: true
hosts:
- cert_expires: Dec 11 05:23:35 2026 GMT
  host: qitech.com.br
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Qi Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QI Tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: QI Tech
provider_slug: qi-tech
slug: qi-tech-domain-security
source_filename: qi-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qitech.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 05:23:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: qitech.com.br\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/qi-tech/security/qi-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Banking as a Service
- Lending
- Payments
- Pix
- KYC
- Fraud Prevention
- Fund Administration
- Brazil
---
