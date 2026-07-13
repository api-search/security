---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: columbia.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: azure-api.net
  spf: false
hosts:
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: www.columbia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: columbia.portal.azure-api.net
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''columbia.po'
kind: domain-security
layout: security
method: probed
name: Columbia Sportswear Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Columbia Sportswear, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Columbia Sportswear
provider_slug: columbia-sportswear
slug: columbia-sportswear-domain-security
source_filename: columbia-sportswear-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.columbia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: columbia.portal.azure-api.net\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''columbia.po'\n  hsts: null\ndomains:\n- domain: columbia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure-api.net\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/columbia-sportswear/refs/heads/main/security/columbia-sportswear-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apparel
- B2B
- Consumer Management
- Cognitive
- Footwear
- Order Management
- Outdoor
- Product Lifecycle
- Retail
- Fortune 1000
---
