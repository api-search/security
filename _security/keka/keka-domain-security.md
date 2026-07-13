---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Keka HR REST API
  slug: keka-hr-rest-api
  spec_type: OpenAPI
  url: https://apidocs.keka.com/
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: keka.com
  spf: true
hosts:
- host: www.keka.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Oct  2 18:01:14 2026 GMT
  host: developers.keka.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keka Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keka HR, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Keka HR
provider_slug: keka
slug: keka-domain-security
source_filename: keka-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.keka.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: developers.keka.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:01:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: keka.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/security/keka-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HR
- Human Resources
- Payroll
- Attendance
- Leave Management
- Performance Management
- Employee Management
- India
- HRMS
---
