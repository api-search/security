---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: convexfinance.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thegraph.com
  spf: true
hosts:
- cert_expires: Sep  2 12:45:33 2026 GMT
  host: docs.convexfinance.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 05:49:39 2026 GMT
  host: api.thegraph.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Convex Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Convex Finance, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Convex Finance
provider_slug: convex-finance
slug: convex-finance-domain-security
source_filename: convex-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.convexfinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 12:45:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.thegraph.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 05:49:39 2026 GMT\n  hsts: null\ndomains:\n- domain: convexfinance.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: thegraph.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convex-finance/refs/heads/main/security/convex-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- Curve Finance
- Yield Boosting
- Liquidity Mining
- Ethereum
- GraphQL
- The Graph
---
