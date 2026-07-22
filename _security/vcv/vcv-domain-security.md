---
api_specs:
- filename: vcv-openapi.yml
  format: yaml
  label: VCV Open API
  slug: vcv-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/openapi/vcv-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vcv.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vcv.ru
  spf: true
hosts:
- cert_expires: Sep 21 20:52:55 2026 GMT
  host: vcv.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: my.vcv.ai
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
- cert_expires: Nov 25 17:17:27 2026 GMT
  host: my.vcv.ru
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vcv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VCV, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VCV
provider_slug: vcv
slug: vcv-domain-security
source_filename: vcv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vcv.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 20:52:55 2026 GMT\n  hsts: false\n- host: my.vcv.ai\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\n- host: my.vcv.ru\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 17:17:27 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: vcv.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: vcv.ru\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vcv/refs/heads/main/security/vcv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recruiting
- Human Resources
- Video Interviews
- Talent Acquisition
- Hiring
- Assessments
---
