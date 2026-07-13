---
api_specs:
- filename: api.github.com.json
  format: json
  label: GitHub Actions API
  slug: github-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/github/rest-api-description/main/descriptions/api.github.com/api.github.com.json
- filename: openapi.json
  format: json
  label: CircleCI API
  slug: circleci-api
  spec_type: OpenAPI
  url: https://circleci.com/api/v2/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: circleci.com
  spf: true
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jenkins.io
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: circleci.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 21:52:45 2026 GMT
  host: www.jenkins.io
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  9 16:14:33 2026 GMT
  host: docs.sonarsource.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Test Driven Development Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Test-Driven Development, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Test-Driven Development
provider_slug: test-driven-development
slug: test-driven-development-domain-security
source_filename: test-driven-development-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: circleci.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.jenkins.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 19 21:52:45 2026 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: docs.sonarsource.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 16:14:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: circleci.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: jenkins.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/test-driven-development/refs/heads/main/security/test-driven-development-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agile
- Best Practices
- Continuous Integration
- Extreme Programming
- Methodology
- Software Development
- Testing
---
