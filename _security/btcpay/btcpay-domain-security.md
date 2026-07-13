---
api_specs:
- filename: openapi.json
  format: json
  label: BTCPay Server Greenfield API
  slug: btcpay-server-greenfield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/btcpay/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: btcpayserver.org
  spf: true
hosts:
- cert_expires: Sep 29 08:22:51 2026 GMT
  host: btcpayserver.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 18:56:19 2026 GMT
  host: docs.btcpayserver.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Btcpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BTCPay Server, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BTCPay Server
provider_slug: btcpay
slug: btcpay-domain-security
source_filename: btcpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: btcpayserver.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 08:22:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: docs.btcpayserver.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:56:19 2026 GMT\n  hsts: false\ndomains:\n- domain: btcpayserver.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/btcpay/refs/heads/main/security/btcpay-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Bitcoin
- Cryptocurrency
- Payments
- Lightning Network
- Open Source
- Self-Hosted
---
