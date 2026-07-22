---
api_specs:
- filename: top-group-tonapi-openapi.yml
  format: yaml
  label: TON API
  slug: tonapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/top-group/refs/heads/main/openapi/top-group-tonapi-openapi.yml
- filename: top-group-tonapi-webhooks-openapi.yml
  format: yaml
  label: TON API Webhooks API
  slug: tonapi-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/top-group/refs/heads/main/openapi/top-group-tonapi-webhooks-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: top.co
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: tonapi.io
  spf: true
hosts:
- cert_expires: Jul 26 12:13:20 2026 GMT
  host: top.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 11:41:16 2026 GMT
  host: tonapi.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 14:47:41 2026 GMT
  host: docs.tonconsole.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Top Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TOP Group (The Open Platform), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TOP Group (The Open Platform)
provider_slug: top-group
slug: top-group-domain-security
source_filename: top-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: top.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 26 12:13:20 2026 GMT\n  hsts: false\n- host: tonapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:41:16 2026 GMT\n  hsts: false\n- host: docs.tonconsole.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 14:47:41 2026 GMT\n  hsts: false\ndomains:\n- domain: top.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tonapi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/top-group/refs/heads/main/security/top-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Blockchain
- TON
- Telegram
- Crypto
- Wallets
- Web3
- NFT
- Payments
---
