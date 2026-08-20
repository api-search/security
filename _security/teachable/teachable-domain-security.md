---
api_specs:
- filename: teachable-courses-api-openapi.yml
  format: yaml
  label: Teachable Courses API
  slug: teachable-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-courses-api-openapi.yml
- filename: teachable-currentuser-api-openapi.yml
  format: yaml
  label: Teachable CurrentUser API
  slug: teachable-currentuser-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-currentuser-api-openapi.yml
- filename: teachable-enrollments-api-openapi.yml
  format: yaml
  label: Teachable Enrollments API
  slug: teachable-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-enrollments-api-openapi.yml
- filename: teachable-lectures-api-openapi.yml
  format: yaml
  label: Teachable Lectures API
  slug: teachable-lectures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-lectures-api-openapi.yml
- filename: teachable-pricingplans-api-openapi.yml
  format: yaml
  label: Teachable PricingPlans API
  slug: teachable-pricingplans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-pricingplans-api-openapi.yml
- filename: teachable-quizzes-api-openapi.yml
  format: yaml
  label: Teachable Quizzes API
  slug: teachable-quizzes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-quizzes-api-openapi.yml
- filename: teachable-transactions-api-openapi.yml
  format: yaml
  label: Teachable Transactions API
  slug: teachable-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-transactions-api-openapi.yml
- filename: teachable-users-api-openapi.yml
  format: yaml
  label: Teachable Users API
  slug: teachable-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-users-api-openapi.yml
- filename: teachable-videos-api-openapi.yml
  format: yaml
  label: Teachable Videos API
  slug: teachable-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-videos-api-openapi.yml
- filename: teachable-webhooks-api-openapi.yml
  format: yaml
  label: Teachable Webhooks API
  slug: teachable-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teachable/refs/heads/main/openapi/teachable-webhooks-api-openapi.yml
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
- Transaction
---
