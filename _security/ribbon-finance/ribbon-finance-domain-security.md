---
api_specs:
- filename: aevo-public-rest-api.json
  format: json
  label: Aevo Exchange Public REST API
  slug: aevo-exchange-public-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-finance/refs/heads/main/openapi/aevo-public-rest-api.json
- filename: aevo-private-rest-api.json
  format: json
  label: Aevo Exchange Private REST API
  slug: aevo-exchange-private-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ribbon-finance/refs/heads/main/openapi/aevo-private-rest-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ribbon.finance
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aevo.xyz
  spf: false
hosts:
- cert_expires: Sep 25 02:47:19 2026 GMT
  host: www.ribbon.finance
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 11:02:20 2026 GMT
  host: api-docs.aevo.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: api.aevo.xyz
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ribbon Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ribbon Finance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ribbon Finance
provider_slug: ribbon-finance
slug: ribbon-finance-domain-security
source_filename: ribbon-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ribbon.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 02:47:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api-docs.aevo.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 11:02:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.aevo.xyz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ribbon.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: aevo.xyz\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ribbon-finance/refs/heads/main/security/ribbon-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DeFi
- Finance
- Options
- Structured Products
- Ethereum
- Layer 2
- Vaults
- Perpetuals
- Yield
---
