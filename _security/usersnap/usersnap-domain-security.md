---
api_specs:
- filename: usersnap-feedback-api-openapi.yml
  format: yaml
  label: Usersnap feedback API
  slug: usersnap-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usersnap/refs/heads/main/openapi/usersnap-feedback-api-openapi.yml
- filename: usersnap-pre-submit-api-openapi.yml
  format: yaml
  label: Usersnap pre_submit API
  slug: usersnap-pre-submit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usersnap/refs/heads/main/openapi/usersnap-pre-submit-api-openapi.yml
- filename: usersnap-project-api-openapi.yml
  format: yaml
  label: Usersnap project API
  slug: usersnap-project-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usersnap/refs/heads/main/openapi/usersnap-project-api-openapi.yml
- filename: usersnap-submit-api-openapi.yml
  format: yaml
  label: Usersnap submit API
  slug: usersnap-submit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/usersnap/refs/heads/main/openapi/usersnap-submit-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: usersnap.com
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: usersnap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  3 22:51:47 2026 GMT
  host: help.usersnap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: platform.usersnap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Usersnap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Usersnap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Usersnap
provider_slug: usersnap
slug: usersnap-domain-security
source_filename: usersnap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usersnap.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.usersnap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 22:51:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.usersnap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: usersnap.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usersnap/refs/heads/main/security/usersnap-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Feedback
- Bug Tracking
- Customer Experience
- Product Management
- Surveys
- Software-as-a-Service
---
