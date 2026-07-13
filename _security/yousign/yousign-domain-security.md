---
api_specs:
- filename: 6759d057a53fa9006fec9ff0
  format: yaml
  label: Yousign Public API v3
  slug: yousign-public-api-v3
  spec_type: OpenAPI
  url: https://developers.yousign.com/openapi/6759d057a53fa9006fec9ff0
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: yousign.com
  spf: true
hosts:
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: yousign.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 06:16:54 2026 GMT
  host: developers.yousign.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  6 17:57:12 2027 GMT
  host: api.yousign.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yousign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YouSign, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: YouSign
provider_slug: yousign
slug: yousign-domain-security
source_filename: yousign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yousign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: false\n- host: developers.yousign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 06:16:54 2026 GMT\n  hsts: null\n- host: api.yousign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  6 17:57:12 2027 GMT\n  hsts: null\ndomains:\n- domain: yousign.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yousign/refs/heads/main/security/yousign-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- E-Signature
- Electronic Signature
- eIDAS
- Digital Signature
- Document Signing
- Europe
- REST API
- Signature Workflows
---
