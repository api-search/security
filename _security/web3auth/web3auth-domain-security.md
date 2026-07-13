---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: web3auth.io
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: web3auth.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 23:59:59 2026 GMT
  host: api.web3auth.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Web3Auth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Web3Auth, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Web3Auth
provider_slug: web3auth
slug: web3auth-domain-security
source_filename: web3auth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: web3auth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: false\n- host: api.web3auth.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: web3auth.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/web3auth/refs/heads/main/security/web3auth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Web3
- Wallets
- Authentication
- MPC
- Embedded Wallets
---
