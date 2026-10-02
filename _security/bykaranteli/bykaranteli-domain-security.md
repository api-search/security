---
api_specs:
- filename: bykaranteli-x402-api-openapi.yml
  format: yaml
  label: ByKaranteli X402 API
  slug: bykaranteli-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bykaranteli/refs/heads/main/openapi/bykaranteli-x402-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bykaranteli.com
  spf: true
hosts:
- cert_expires: Nov 18 20:51:38 2026 GMT
  host: www.bykaranteli.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 20:51:38 2026 GMT
  host: bykaranteli.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Bykaranteli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ByKaranteli, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ByKaranteli
provider_slug: bykaranteli
slug: bykaranteli-domain-security
source_filename: bykaranteli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bykaranteli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 20:51:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: bykaranteli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 20:51:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bykaranteli.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bykaranteli/refs/heads/main/security/bykaranteli-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cryptocurrency
- Crypto Derivatives
- Market Data
- Funding Rates
- Open Interest
- Liquidations
- Options
- ETF Flows
- Financial Data
- MCP
- x402
- Agents
---
