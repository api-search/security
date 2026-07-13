---
api_specs:
- filename: thinkific-admin-api-openapi.yml
  format: yaml
  label: Thinkific Admin REST API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thinkific/refs/heads/main/openapi/thinkific-admin-api-openapi.yml
- filename: thinkific-webhooks-api-openapi.yml
  format: yaml
  label: Thinkific Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thinkific/refs/heads/main/openapi/thinkific-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thinkific.com
  spf: true
hosts:
- cert_expires: Aug 28 05:27:40 2026 GMT
  host: www.thinkific.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: developers.thinkific.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 18:27:00 2026 GMT
  host: api.thinkific.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thinkific Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Thinkific, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Thinkific
provider_slug: thinkific
slug: thinkific-domain-security
source_filename: thinkific-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thinkific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 05:27:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.thinkific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\n- host: api.thinkific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 18:27:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thinkific.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thinkific/refs/heads/main/security/thinkific-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Online Courses
- E-Learning
- LMS
- Course Creation
- Enrollments
- Users
- Education
- Digital Products
- Webhooks
---
