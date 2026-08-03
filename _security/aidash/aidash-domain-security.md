---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: aidash.com
  spf: true
hosts:
- cert_expires: Oct  8 01:04:14 2026 GMT
  host: connect.aidash.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: evolve.aidash.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Sep 16 20:00:10 2026 GMT
  host: iris.aidash.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: security.aidash.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: www.aidash.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aidash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AiDASH, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AiDASH
provider_slug: aidash
slug: aidash-domain-security
source_filename: aidash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: connect.aidash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:04:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: evolve.aidash.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable\n    to get local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: iris.aidash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 20:00:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: security.aidash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: null\n- host: www.aidash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: aidash.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aidash/refs/heads/main/security/aidash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Satellite
- Artificial Intelligence
- Geospatial
- Utilities
- Energy
- Vegetation Management
- Wildfire
- Climate Risk
- Asset Management
- Remote Sensing
- Vertical SaaS
---
