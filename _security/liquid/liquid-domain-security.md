---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: tryliquid.xyz
  spf: true
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: liquid.trade
  spf: true
hosts:
- cert_expires: Aug 22 18:38:22 2026 GMT
  host: tryliquid.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 23:47:22 2026 GMT
  host: www.liquid.trade
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 16:48:38 2026 GMT
  host: coinvest.liquid.trade
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liquid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liquid, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Liquid
provider_slug: liquid
slug: liquid-domain-security
source_filename: liquid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tryliquid.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 18:38:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.liquid.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 23:47:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: coinvest.liquid.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 16:48:38 2026 GMT\n  hsts: null\ndomains:\n- domain: tryliquid.xyz\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: liquid.trade\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  -\
  \ 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquid/refs/heads/main/security/liquid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Defi
- Trading
- Perpetual Futures
- Prediction Markets
- Fintech
- MCP
- Agentic Commerce
- OAuth
---
