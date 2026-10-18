---
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: augment.market
  spf: true
hosts:
- cert_expires: Dec 13 09:02:24 2026 GMT
  host: augment.market
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ctristack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ctristack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ctristack
provider_slug: ctristack
slug: ctristack-domain-security
source_filename: ctristack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: augment.market\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 09:02:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: augment.market\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ctristack/refs/heads/main/security/ctristack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- PrivateLiquidity
- Market Data
- Investor
- TradingPlatform
---
