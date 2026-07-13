---
api_specs:
- filename: gitcoin-core-api-openapi.json
  format: json
  label: Gitcoin Core API
  slug: gitcoin-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitcoin/refs/heads/main/openapi/gitcoin-core-api-openapi.json
- filename: gitcoin-grants-api-openapi.json
  format: json
  label: Gitcoin Grants API
  slug: gitcoin-grants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitcoin/refs/heads/main/openapi/gitcoin-grants-api-openapi.json
- filename: gitcoin-passport-stamps-api-openapi.json
  format: json
  label: Gitcoin Passport Stamps API
  slug: gitcoin-passport-stamps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gitcoin/refs/heads/main/openapi/gitcoin-passport-stamps-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitcoin.co
  spf: true
hosts:
- cert_expires: Sep 23 12:41:40 2026 GMT
  host: gitcoin.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: docs.gitcoin.co
  https: false
- host: grants-stack-indexer-v2.gitcoin.co
  https: false
kind: domain-security
layout: security
method: probed
name: Gitcoin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gitcoin, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gitcoin
provider_slug: gitcoin
slug: gitcoin-domain-security
source_filename: gitcoin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gitcoin.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 12:41:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.gitcoin.co\n  https: false\n- host: grants-stack-indexer-v2.gitcoin.co\n  https: false\ndomains:\n- domain: gitcoin.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitcoin/refs/heads/main/security/gitcoin-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Public Goods
- Grants
- Bounties
- Quadratic Funding
- Web3
- Verifiable Credentials
- Identity
- Open Source
---
