---
api_specs:
- filename: openwallet-foundation-openapi.yml
  format: yaml
  label: ACA-Py Admin API
  slug: aca-py-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openwallet-foundation/refs/heads/main/openapi/openwallet-foundation-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openwallet.foundation
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: aca-py.org
  spf: false
hosts:
- cert_expires: Aug 27 19:15:50 2026 GMT
  host: openwallet.foundation
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 21:37:21 2026 GMT
  host: aca-py.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 14:27:59 2026 GMT
  host: credo.js.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openwallet Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenWallet Foundation, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OpenWallet Foundation
provider_slug: openwallet-foundation
slug: openwallet-foundation-domain-security
source_filename: openwallet-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openwallet.foundation\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: aca-py.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 21:37:21 2026 GMT\n  hsts: false\n- host: credo.js.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 14:27:59 2026 GMT\n  hsts: false\ndomains:\n- domain: openwallet.foundation\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: aca-py.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openwallet-foundation/refs/heads/main/security/openwallet-foundation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Credentials
- Digital Wallet
- Identity
- Linux Foundation
---
