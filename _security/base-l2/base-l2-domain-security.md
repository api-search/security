---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: base.org
  spf: true
hosts:
- cert_expires: Aug 24 08:27:22 2026 GMT
  host: www.base.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 03:32:48 2026 GMT
  host: docs.base.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 08:27:22 2026 GMT
  host: mainnet.base.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Base L2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Base, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Base
provider_slug: base-l2
slug: base-l2-domain-security
source_filename: base-l2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.base.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:27:22 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.base.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:32:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mainnet.base.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:27:22 2026 GMT\n  hsts: null\ndomains:\n- domain: base.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/base-l2/refs/heads/main/security/base-l2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Layer 2
- Ethereum
- OP Stack
- Superchain
- JSON-RPC
- Smart Wallet
- Bridge
---
