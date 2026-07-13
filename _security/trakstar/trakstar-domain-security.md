---
api_specs:
- filename: trakstar-hire-api-openapi.yml
  format: yaml
  label: Trakstar Hire API
  slug: trakstar-hire-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-hire-api-openapi.yml
- filename: trakstar-learn-api-openapi.yml
  format: yaml
  label: Trakstar Learn API
  slug: trakstar-learn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-learn-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: trakstar.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: recruiterbox.com
  spf: true
hosts:
- cert_expires: Sep 26 08:47:54 2026 GMT
  host: www.trakstar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 15:13:29 2026 GMT
  host: developers.recruiterbox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: companyname.hire.trakstar.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Trakstar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trakstar, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Trakstar
provider_slug: trakstar
slug: trakstar-domain-security
source_filename: trakstar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trakstar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 08:47:54 2026 GMT\n  hsts: false\n- host: developers.recruiterbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 15:13:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: companyname.hire.trakstar.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: trakstar.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: recruiterbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/security/trakstar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- Human Resources
- Performance Management
- Talent Management
- Applicant Tracking
- Learning Management
- 360 Feedback
- Goal Management
- Employee Development
- Performance Appraisal
---
