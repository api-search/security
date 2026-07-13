---
api_specs:
- filename: al-farabi-kazakh-national-university-open-edx.yaml
  format: yaml
  label: KazNU Open edX API
  slug: kaznu-open-edx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/al-farabi-kazakh-national-university/refs/heads/main/openapi/al-farabi-kazakh-national-university-open-edx.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: farabi.university
  spf: false
- caa: []
  dmarc: false
  dnssec: false
  domain: kaznu.kz
  spf: true
hosts:
- host: farabi.university
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- host: www.kaznu.kz
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
- host: open.kaznu.kz
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Al Farabi Kazakh National University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Al-Farabi Kazakh National University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Al-Farabi Kazakh National University
provider_slug: al-farabi-kazakh-national-university
slug: al-farabi-kazakh-national-university-domain-security
source_filename: al-farabi-kazakh-national-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: farabi.university\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: www.kaznu.kz\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\n- host: open.kaznu.kz\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: farabi.university\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: kaznu.kz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/al-farabi-kazakh-national-university/refs/heads/main/security/al-farabi-kazakh-national-university-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Education
- Higher Education
- University
- Research
- Library
- Open Education
- Kazakhstan
- Central Asia
---
