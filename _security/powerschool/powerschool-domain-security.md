---
api_specs:
- filename: powerschool-powerschool-sis-api-openapi.yml
  format: yaml
  label: PowerSchool SIS REST API
  slug: powerschool-sis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powerschool/refs/heads/main/openapi/powerschool-powerschool-sis-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: powerschool.com
  spf: true
hosts:
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: www.powerschool.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 23:59:59 2026 GMT
  host: support.powerschool.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Powerschool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PowerSchool, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PowerSchool
provider_slug: powerschool
slug: powerschool-domain-security
source_filename: powerschool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.powerschool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: support.powerschool.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: powerschool.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powerschool/refs/heads/main/security/powerschool-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- K-12
- Education
- Student Information System
- SIS
- Students
- Grades
- Attendance
- Enrollment
- Scheduling
- EdTech
---
