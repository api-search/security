---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crossingminds.com
  spf: true
hosts:
- cert_expires: Sep 26 07:57:26 2026 GMT
  host: www.crossingminds.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: docs.api.crossingminds.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.crossingminds.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''api.crossin'
kind: domain-security
layout: security
method: probed
name: Crossing Minds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crossing Minds, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crossing Minds
provider_slug: crossing-minds
slug: crossing-minds-domain-security
source_filename: crossing-minds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crossingminds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 07:57:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.api.crossingminds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: false\n- host: api.crossingminds.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''api.crossin'\n  hsts: null\ndomains:\n- domain: crossingminds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossing-minds/refs/heads/main/security/crossing-minds-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Recommendations
- Personalization
- Machine Learning
- Recommender System
- Retrieval
- Ecommerce
---
