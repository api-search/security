---
api_specs:
- filename: texas-instruments-store-openapi.yml
  format: yaml
  label: Texas Instruments Store API
  slug: ti-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/openapi/texas-instruments-store-openapi.yml
- filename: texas-instruments-product-information-openapi.yml
  format: yaml
  label: Texas Instruments Product Information API
  slug: ti-product-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/openapi/texas-instruments-product-information-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: texas-instruments.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ti.com
  spf: true
hosts:
- host: www.texas-instruments.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.texas-i'
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: www.ti.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: transact.ti.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Texas Instruments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Texas Instruments, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Texas Instruments
provider_slug: texas-instruments
slug: texas-instruments-domain-security
source_filename: texas-instruments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.texas-instruments.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.texas-i'\n  hsts: null\n- host: www.ti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: transact.ti.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: texas-instruments.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: ti.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/security/texas-instruments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Electronics
- Ordering
- Semiconductors
- Supply Chain
- Fortune 500
---
