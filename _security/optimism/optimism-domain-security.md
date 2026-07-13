---
api_specs:
- filename: optimism-asyncapi.yml
  format: yaml
  label: OP Mainnet JSON-RPC
  slug: mainnet-rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimism/refs/heads/main/asyncapi/optimism-asyncapi.yml
- filename: optimism-asyncapi.yml
  format: yaml
  label: OP Sepolia JSON-RPC
  slug: sepolia-rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimism/refs/heads/main/asyncapi/optimism-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: optimism.io
  spf: true
hosts:
- cert_expires: Aug 20 20:53:43 2026 GMT
  host: www.optimism.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 15:11:25 2026 GMT
  host: docs.optimism.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 00:00:16 2026 GMT
  host: mainnet.optimism.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Optimism Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Optimism, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Optimism
provider_slug: optimism
slug: optimism-domain-security
source_filename: optimism-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.optimism.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 20:53:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.optimism.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 15:11:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mainnet.optimism.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 00:00:16 2026 GMT\n  hsts: null\ndomains:\n- domain: optimism.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optimism/refs/heads/main/security/optimism-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Layer 2
- Ethereum
- OP Stack
- Superchain
- JSON-RPC
- Rollup
- Bridge
---
