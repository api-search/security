---
api_specs:
- filename: import2-openapi.yml
  format: yaml
  label: Import2 API
  slug: import2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/import2/refs/heads/main/openapi/import2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: import2.com
  spf: true
hosts:
- cert_expires: Oct 13 23:21:02 2026 GMT
  host: import2.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.import2.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Import2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Import2, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Import2
provider_slug: import2
slug: import2-domain-security
source_filename: import2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: import2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:21:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.import2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: import2.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/import2/refs/heads/main/security/import2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data Migration
- Data Integration
- CRM
- Helpdesk
- SaaS
- Migration
- Onboarding
---
