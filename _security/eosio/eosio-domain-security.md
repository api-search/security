---
api_specs:
- filename: eosio-nodeos-chain-api-openapi.yml
  format: yaml
  label: EOSIO Nodeos Chain API
  slug: nodeos-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eosio/refs/heads/main/openapi/eosio-nodeos-chain-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eosnetwork.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eos.io
  spf: true
hosts:
- cert_expires: Aug 25 20:35:10 2026 GMT
  host: eosnetwork.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 15:33:42 2026 GMT
  host: developers.eos.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eosio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EOSIO, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EOSIO
provider_slug: eosio
slug: eosio-domain-security
source_filename: eosio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eosnetwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 20:35:10 2026 GMT\n  hsts: null\n- host: developers.eos.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 15:33:42 2026 GMT\n  hsts: null\ndomains:\n- domain: eosnetwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: eos.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eosio/refs/heads/main/security/eosio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Antelope
- Blockchain
- EOS
---
