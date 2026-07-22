---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: vault12.com
  spf: true
hosts:
- cert_expires: Sep  8 21:12:16 2026 GMT
  host: vault12.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 16:11:31 2026 GMT
  host: zt.vault12.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vault12 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vault12, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Vault12
provider_slug: vault12
slug: vault12-domain-security
source_filename: vault12-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vault12.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 21:12:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: zt.vault12.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 16:11:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vault12.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vault12/refs/heads/main/security/vault12-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Security
- Backup
- Inheritance
- Wallets
- Cryptography
- Secret Sharing
- Key Management
---
