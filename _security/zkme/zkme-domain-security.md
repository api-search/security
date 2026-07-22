---
api_specs:
- filename: zkme-openapi.yml
  format: yaml
  label: zkMe Protocol API
  slug: zkme-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zkme/refs/heads/main/openapi/zkme-openapi.yml
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
  dmarc_policy: reject
  dnssec: true
  domain: zk.me
  spf: true
hosts:
- cert_expires: Sep 15 14:55:36 2026 GMT
  host: zk.me
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 18:15:37 2026 GMT
  host: docs.zk.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 14:55:36 2026 GMT
  host: agw.zk.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zkme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for zkMe, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: zkMe
provider_slug: zkme
slug: zkme-domain-security
source_filename: zkme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zk.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:55:36 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.zk.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 18:15:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: agw.zk.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 14:55:36 2026 GMT\n  hsts: null\ndomains:\n- domain: zk.me\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zkme/refs/heads/main/security/zkme-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- Identity
- KYC
- KYB
- Compliance
- Zero Knowledge
- Decentralized Identity
- Anti-Sybil
- Transaction Monitoring
---
