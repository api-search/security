---
api_specs:
- filename: survicate-data-export-openapi.yml
  format: yaml
  label: Survicate Data Export API
  slug: survicate-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/survicate/refs/heads/main/openapi/survicate-data-export-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: survicate.com
  spf: true
hosts:
- cert_expires: Sep 25 23:59:59 2026 GMT
  host: survicate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 04:31:17 2026 GMT
  host: developers.survicate.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- host: data.survicate.com
  https: false
kind: domain-security
layout: security
method: probed
name: Survicate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Survicate, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Survicate
provider_slug: survicate
slug: survicate-domain-security
source_filename: survicate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: survicate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.survicate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 04:31:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: data.survicate.com\n  https: false\ndomains:\n- domain: survicate.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/survicate/refs/heads/main/security/survicate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Surveys
- Customer Feedback
- NPS
- User Research
- Feedback Analytics
- CRM Integration
- Customer Experience
---
