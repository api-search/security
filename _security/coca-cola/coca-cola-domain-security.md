---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coca-colacompany.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mulesoft.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.coca-colacompany.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: www.mulesoft.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- host: developer.cokecce.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''developer.c'
kind: domain-security
layout: security
method: probed
name: Coca Cola Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Coca-Cola Company, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: The Coca-Cola Company
provider_slug: coca-cola
slug: coca-cola-domain-security
source_filename: coca-cola-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coca-colacompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.mulesoft.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.cokecce.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''developer.c'\n  hsts: null\ndomains:\n- domain: coca-colacompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mulesoft.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coca-cola/refs/heads/main/security/coca-cola-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Beverages
- Beverage Manufacturer
- Consumer Goods
- Distribution
- Retail
- Supply Chain
---
