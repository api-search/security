---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: liesheng.cc
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: suunto.com
  spf: true
hosts:
- host: liesheng.cc
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''liesheng.cc'
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: apizone.suunto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: cloudapi.suunto.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liesheng Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liesheng Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Liesheng Group
provider_slug: liesheng
slug: liesheng-domain-security
source_filename: liesheng-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liesheng.cc\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''liesheng.cc'\n  hsts: null\n- host: apizone.suunto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: cloudapi.suunto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: liesheng.cc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: suunto.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liesheng/refs/heads/main/security/liesheng-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Electronics
- Wearables
- Audio
- Sports
- Fitness
- Health
- Internet of Things
- ODM
- OEM
- China
---
