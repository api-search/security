---
api_specs:
- filename: bakkt-crypto-openapi.yml
  format: yaml
  label: Bakkt Crypto Solutions API
  slug: bakkt-crypto-solutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/openapi/bakkt-crypto-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bakkt.com
  spf: true
hosts:
- cert_expires: Oct  6 13:18:19 2026 GMT
  host: bakkt.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bakkt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bakkt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bakkt
provider_slug: bakkt
slug: bakkt-domain-security
source_filename: bakkt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bakkt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 13:18:19 2026 GMT\n  hsts: false\ndomains:\n- domain: bakkt.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bakkt/refs/heads/main/security/bakkt-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- Cryptocurrency
- Digital Assets
- Trading
- Payments
- Fiat On-Ramp
- Custody
- Webhooks
- FIX Protocol
---
