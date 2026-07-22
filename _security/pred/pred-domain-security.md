---
api_specs:
- filename: pred-openapi.yml
  format: yaml
  label: PRED Trading Platform API
  slug: pred-trading-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pred/refs/heads/main/openapi/pred-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pred.app
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitbook.io
  spf: true
hosts:
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: www.pred.app
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 19:03:12 2026 GMT
  host: pred-1.gitbook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: testnet.pred.app
  https: false
kind: domain-security
layout: security
method: probed
name: Pred Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pred, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pred
provider_slug: pred
slug: pred-domain-security
source_filename: pred-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pred.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: null\n- host: pred-1.gitbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 19:03:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: testnet.pred.app\n  https: false\ndomains:\n- domain: pred.app\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gitbook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pred/refs/heads/main/security/pred-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Prediction Markets
- Sports
- Trading
- Exchange
- Web3
- Blockchain
- Base
- USDC
---
