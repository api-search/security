---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: genesis.global
  spf: true
hosts:
- cert_expires: Jan 15 15:20:12 2027 GMT
  host: genesis.global
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Genesis Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genesis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Genesis
provider_slug: genesis-global
slug: genesis-global-domain-security
source_filename: genesis-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genesis.global\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 15:20:12 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: genesis.global\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/genesis-global/security/genesis-global-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Architecture
- Capital Markets
- Financial Institutions
- Developer Portal
- Trading Platforms
- Middle Office
- Electronic Trading
---
