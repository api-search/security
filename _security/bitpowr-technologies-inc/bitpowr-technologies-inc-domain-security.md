---
api_specs:
- filename: bitpowr-technologies-inc-openapi.yml
  format: yaml
  label: Bitpowr Developer API
  slug: bitpowr-developer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitpowr-technologies-inc/refs/heads/main/openapi/bitpowr-technologies-inc-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bitpowr.com
  spf: true
hosts:
- cert_expires: Sep 17 03:05:30 2026 GMT
  host: bitpowr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 03:05:30 2026 GMT
  host: developers.bitpowr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitpowr Technologies Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BitPowr Technologies, Inc., probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BitPowr Technologies, Inc.
provider_slug: bitpowr-technologies-inc
slug: bitpowr-technologies-inc-domain-security
source_filename: bitpowr-technologies-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitpowr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 03:05:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.bitpowr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 03:05:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bitpowr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitpowr-technologies-inc/refs/heads/main/security/bitpowr-technologies-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cryptocurrency
- Blockchain
- Digital Assets
- Wallet Infrastructure
- Wallet as a Service
- Custody
- Treasury Management
- Tokenization
- Compliance
- Web3
- Payments
---
