---
api_specs:
- filename: openapi
  format: yaml
  label: Velocity Global API
  slug: velocity-global-api
  spec_type: OpenAPI
  url: https://velocityglobal.com/openapi
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: velocityglobal.com
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: velocityglobal.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: api.velocityglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Velocity Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Velocity Global, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Velocity Global
provider_slug: velocity-global
slug: velocity-global-domain-security
source_filename: velocity-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: velocityglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: api.velocityglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: velocityglobal.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/velocity-global/refs/heads/main/security/velocity-global-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- EOR
- Employer of Record
- Global Employment
- HR
- Payroll
- Compliance
- International Hiring
- Workforce Management
---
