---
api_specs:
- filename: teachable-admin-openapi.yml
  format: yaml
  label: Teachable Admin API
  slug: teachable-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-admin-openapi.yml
- filename: teachable-oauth-openapi.yml
  format: yaml
  label: Teachable OAuth API
  slug: teachable-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-oauth-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: teachable.com
  spf: true
hosts:
- cert_expires: Aug 28 02:22:17 2026 GMT
  host: teachable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 08:53:09 2026 GMT
  host: docs.teachable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 11:16:00 2026 GMT
  host: developers.teachable.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teachable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teachable, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Teachable
provider_slug: teachable
slug: teachable-domain-security
source_filename: teachable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teachable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 02:22:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.teachable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:53:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.teachable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 11:16:00 2026 GMT\n  hsts: null\ndomains:\n- domain: teachable.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/security/teachable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Online Courses
- E-Learning
- Education
- Course Management
- Enrollments
- Coaching
- Memberships
- Transactions
---
