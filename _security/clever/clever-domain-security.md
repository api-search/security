---
api_specs:
- filename: clever-data-api-openapi.yml
  format: yaml
  label: Clever Data API
  slug: clever-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-data-api-openapi.yml
- filename: clever-lms-connect-api-openapi.yml
  format: yaml
  label: Clever LMS Connect API
  slug: clever-lms-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-lms-connect-api-openapi.yml
- filename: clever-events-api-openapi.yml
  format: yaml
  label: Clever Events API
  slug: clever-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-events-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clever.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: clever.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 09:16:22 2026 GMT
  host: dev.clever.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.clever.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Clever Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clever, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clever
provider_slug: clever
slug: clever-domain-security
source_filename: clever-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clever.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n- host: dev.clever.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 09:16:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.clever.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: clever.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/security/clever-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- K-12
- EdTech
- Single Sign-On
- Rostering
- Identity
- SSO
- Student Data
- LMS
- SIS
---
