---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Nano RPC API - Account Operations
  slug: nano-rpc-api-account-operations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nano/refs/heads/main/openapi.yml
- filename: openapi.yml
  format: yaml
  label: Nano RPC API - Block Operations
  slug: nano-rpc-api-block-operations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nano/refs/heads/main/openapi.yml
- filename: openapi.yml
  format: yaml
  label: Nano RPC API - Node Operations
  slug: nano-rpc-api-node-operations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nano/refs/heads/main/openapi.yml
- filename: openapi.yml
  format: yaml
  label: Nano RPC API - Wallet Operations
  slug: nano-rpc-api-wallet-operations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nano/refs/heads/main/openapi.yml
- filename: openapi.yml
  format: yaml
  label: Nano RPC API - Unit Conversion
  slug: nano-rpc-api-unit-conversion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nano/refs/heads/main/openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nano.org
  spf: true
hosts:
- cert_expires: Sep 28 17:01:15 2026 GMT
  host: nano.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 05:23:48 2026 GMT
  host: docs.nano.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nano Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nano, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nano
provider_slug: nano
slug: nano-domain-security
source_filename: nano-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nano.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:01:15 2026 GMT\n  hsts: false\n- host: docs.nano.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 05:23:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: nano.org\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nano/refs/heads/main/security/nano-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Payments
- Blockchain
- Feeless
- Instant Payments
- Digital Currency
---
