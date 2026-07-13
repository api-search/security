---
api_specs:
- filename: litecoin-core-json-rpc.yml
  format: yaml
  label: Litecoin Core JSON-RPC API
  slug: litecoin-core-json-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/openapi/litecoin-core-json-rpc.yml
- filename: litecoin-core-rest.yml
  format: yaml
  label: Litecoin Core REST API
  slug: litecoin-core-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/openapi/litecoin-core-rest.yml
- filename: litecoin-space-rest.yml
  format: yaml
  label: Litecoin Space REST API
  slug: litecoin-space-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/openapi/litecoin-space-rest.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: litecoin.org
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: true
  domain: litecoinspace.org
  spf: false
hosts:
- cert_expires: Oct  3 20:49:12 2026 GMT
  host: litecoin.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 04:22:10 2026 GMT
  host: litecoinspace.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Litecoin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Litecoin, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Litecoin
provider_slug: litecoin
slug: litecoin-domain-security
source_filename: litecoin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: litecoin.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:49:12 2026 GMT\n  hsts: false\n- host: litecoinspace.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 04:22:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: litecoin.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n- domain: litecoinspace.org\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/litecoin/refs/heads/main/security/litecoin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Cryptocurrency
- Blockchain
- Litecoin
- LTC
- Payments
- Decentralized Finance
- Block Explorer
- JSON-RPC
---
