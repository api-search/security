---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: thundercore.com
  spf: true
hosts:
- cert_expires: Mar  9 23:59:59 2027 GMT
  host: www.thundercore.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 10:24:33 2026 GMT
  host: docs.developers.thundercore.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: mainnet-rpc.thundercore.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Thundercore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThunderCore, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ThunderCore
provider_slug: thundercore
slug: thundercore-domain-security
source_filename: thundercore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thundercore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.developers.thundercore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 10:24:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mainnet-rpc.thundercore.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: thundercore.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thundercore/refs/heads/main/security/thundercore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Blockchain
- EVM
- JSON-RPC
- Web3
- Layer 1
---
