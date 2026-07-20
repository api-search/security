---
api_specs:
- filename: adopets-external-openapi.yml
  format: yaml
  label: Adopets External API
  slug: adopets-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adopets/refs/heads/main/openapi/adopets-external-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adopets.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adopets.app
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: adopets.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: service.api.dev.adopets.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: service.api.adopets.app
  https: false
kind: domain-security
layout: security
method: probed
name: Adopets Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adopets, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Adopets
provider_slug: adopets
slug: adopets-domain-security
source_filename: adopets-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adopets.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: false\n- host: service.api.dev.adopets.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: service.api.adopets.app\n  https: false\ndomains:\n- domain: adopets.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: adopets.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adopets/refs/heads/main/security/adopets-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pet Adoption
- Animal Welfare
- Shelters and Rescues
- Adoption Management
- Payments
- Nonprofit Technology
- SaaS
- Company
---
