---
api_specs:
- filename: octav-openapi-original.json
  format: json
  label: Octav API
  slug: octav-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "cloudflare.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: octav.fi
  spf: true
hosts:
- cert_expires: Aug 28 14:41:13 2026 GMT
  host: api.octav.fi
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Octav Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octav, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Octav
provider_slug: octav
slug: octav-domain-security
source_filename: octav-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.octav.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 14:41:13 2026 GMT\n  hsts: null\ndomains:\n- domain: octav.fi\n  dnssec: true\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"cloudflare.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/security/octav-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Blockchain
- Portfolio
- DeFi
- Analytics
- Web3
- Financial Data
- Wallet
---
