---
api_specs:
- filename: zenhr-inc-openapi.yml
  format: yaml
  label: ZenHR API
  slug: zenhr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenhr-inc/refs/heads/main/openapi/zenhr-inc-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issue "trust-provider.com"
  - 0 issue "usertrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zenhr.com
  spf: true
hosts:
- cert_expires: Oct  4 12:18:18 2026 GMT
  host: zenhr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 13:03:32 2026 GMT
  host: app.zenhr.com
  hsts: true
  hsts_max_age: 2678400
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: aiapi.zenhr.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Zenhr Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZenHR Inc, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ZenHR Inc
provider_slug: zenhr-inc
slug: zenhr-inc-domain-security
source_filename: zenhr-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zenhr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 12:18:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.zenhr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 13:03:32 2026 GMT\n  hsts: true\n  hsts_max_age: 2678400\n- host: aiapi.zenhr.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: zenhr.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"trust-provider.com\"\n  - 0 issue \"usertrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenhr-inc/refs/heads/main/security/zenhr-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Human Resources
- HR
- Payroll
- HRMS
- Employee Management
- MENA
- Attendance
- Time Off
- SaaS
---
