---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: acrove.co.jp
  spf: true
hosts:
- cert_expires: Oct 22 03:09:58 2026 GMT
  host: acrove.co.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 12:51:22 2026 GMT
  host: commerce.acrove.co.jp
  hsts: false
  https: true
  note: Magento / Adobe Commerce services site (formerly Digital-Free K.K.); serves the llms.txt captured in llms/.
  server: nginx/1.24.0
  tls_version: TLSv1.3
- cert_expires: Dec  3 05:44:13 2026 GMT
  host: mdm.acrove.co.jp
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Login-gated first-party application "ACROVE MDM". No public API surface; every probed path 404s.
  server: Google Frontend
  tls_version: TLSv1.3
- cert_expires: Oct 17 02:54:04 2026 GMT
  host: kb.acrove.co.jp
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  hsts_preload: true
  https: true
  note: Login-gated first-party application "ACROVE KNOWLEDGE BASE". Every probed path 307s to its login.
  server: Google Frontend
  tls_version: TLSv1.3
hosts_probed: 4
kind: domain-security
layout: security
method: probed
name: Acrove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ACROVE, Inc., probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ACROVE, Inc.
provider_slug: acrove
slug: acrove-domain-security
source_filename: acrove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the apis.yml Website host plus every other host ACROVE, Inc. operates\n  that was found in certificate transparency (commerce.acrove.co.jp, mdm.acrove.co.jp, kb.acrove.co.jp).\n  There are no API baseURL or OpenAPI servers[] hosts to probe — the company publishes no API.\nhosts:\n- host: acrove.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 03:09:58 2026 GMT\n  hsts: false\n- host: commerce.acrove.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 12:51:22 2026 GMT\n  hsts: false\n  server: nginx/1.24.0\n  note: Magento / Adobe Commerce services site (formerly Digital-Free K.K.); serves the llms.txt captured\n    in llms/.\n- host: mdm.acrove.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 05:44:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  server: Google Frontend\n  note: Login-gated first-party\
  \ application \"ACROVE MDM\". No public API surface; every probed path 404s.\n- host: kb.acrove.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 02:54:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  server: Google Frontend\n  note: Login-gated first-party application \"ACROVE KNOWLEDGE BASE\". Every probed path 307s to its login.\ndomains:\n- domain: acrove.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acrove/refs/heads/main/security/acrove-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- E-commerce
- Marketplaces
- Business Intelligence
- Retail
- Consumer Brands
- Adobe Commerce
- Japan
---
