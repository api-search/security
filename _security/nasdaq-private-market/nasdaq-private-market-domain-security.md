---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nasdaqprivatemarket.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nasdaq.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: secondmarket.com
  spf: true
hosts:
- cert_expires: Oct 22 07:26:08 2026 GMT
  host: www.nasdaqprivatemarket.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 02:37:40 2026 GMT
  host: data.nasdaq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: fe.secondmarket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 22:57:24 2026 GMT
  host: fe.login.secondmarket.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Nasdaq Private Market Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nasdaq Private Market, probed live across 4 host(s) and 3 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nasdaq Private Market
provider_slug: nasdaq-private-market
slug: nasdaq-private-market-domain-security
source_filename: nasdaq-private-market-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nasdaqprivatemarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 07:26:08 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: data.nasdaq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 02:37:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fe.secondmarket.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fe.login.secondmarket.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 11 22:57:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nasdaqprivatemarket.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: nasdaq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: secondmarket.com\n  dnssec:\
  \ false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasdaq-private-market/refs/heads/main/security/nasdaq-private-market-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Private Markets
- Secondary Markets
- Market Data
- Financial-Services
- Valuations
- Pre-IPO Equity
- Capital Markets
---
