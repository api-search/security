---
api_specs:
- filename: clever-events-api-openapi.yml
  format: yaml
  label: Clever Events API
  slug: clever-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-events-api-openapi.yml
- filename: clever-assignments-api-openapi.yml
  format: yaml
  label: Clever Assignments API
  slug: clever-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-assignments-api-openapi.yml
- filename: clever-courses-api-openapi.yml
  format: yaml
  label: Clever Courses API
  slug: clever-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-courses-api-openapi.yml
- filename: clever-districts-api-openapi.yml
  format: yaml
  label: Clever Districts API
  slug: clever-districts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-districts-api-openapi.yml
- filename: clever-resources-api-openapi.yml
  format: yaml
  label: Clever Resources API
  slug: clever-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-resources-api-openapi.yml
- filename: clever-schools-api-openapi.yml
  format: yaml
  label: Clever Schools API
  slug: clever-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-schools-api-openapi.yml
- filename: clever-sections-api-openapi.yml
  format: yaml
  label: Clever Sections API
  slug: clever-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-sections-api-openapi.yml
- filename: clever-submissions-api-openapi.yml
  format: yaml
  label: Clever Submissions API
  slug: clever-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-submissions-api-openapi.yml
- filename: clever-terms-api-openapi.yml
  format: yaml
  label: Clever Terms API
  slug: clever-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-terms-api-openapi.yml
- filename: clever-users-api-openapi.yml
  format: yaml
  label: Clever Users API
  slug: clever-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clever/refs/heads/main/openapi/clever-users-api-openapi.yml
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
