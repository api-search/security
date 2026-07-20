---
api_specs:
- filename: activtrak-openapi-original.yaml
  format: yaml
  label: ActivTrak Public APIs
  slug: activtrak-public-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activtrak/refs/heads/main/openapi/activtrak-openapi-original.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: activtrak.com
  spf: true
hosts:
- cert_expires: Nov 27 16:04:46 2026 GMT
  host: www.activtrak.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 22:00:07 2026 GMT
  host: api.activtrak.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 08:20:49 2026 GMT
  host: api-eu.activtrak.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Activtrak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ActivTrak, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ActivTrak
provider_slug: activtrak
slug: activtrak-domain-security
source_filename: activtrak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.activtrak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 16:04:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.activtrak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:00:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-eu.activtrak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 08:20:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: activtrak.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activtrak/refs/heads/main/security/activtrak-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Saas
- Workforce Analytics
- Productivity
- Employee Monitoring
- Workforce Management
- SCIM
- Reporting
---
