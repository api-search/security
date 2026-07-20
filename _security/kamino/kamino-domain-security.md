---
api_specs:
- filename: kamino-public-openapi-original.json
  format: json
  label: Kamino Public API
  slug: kamino-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kamino/refs/heads/main/openapi/kamino-public-openapi-original.json
- filename: kamino-transactions-openapi-original.json
  format: json
  label: Kamino Transactions API
  slug: kamino-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kamino/refs/heads/main/openapi/kamino-transactions-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kamino.finance
  spf: true
hosts:
- cert_expires: Oct 15 00:48:08 2026 GMT
  host: kamino.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 20:11:59 2026 GMT
  host: api.kamino.finance
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kamino Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kamino, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kamino
provider_slug: kamino
slug: kamino-domain-security
source_filename: kamino-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kamino.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 00:48:08 2026 GMT\n  hsts: null\n- host: api.kamino.finance\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 20:11:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kamino.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kamino/refs/heads/main/security/kamino-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- DeFi
- Solana
- Lending
- Borrowing
- Yield
- Blockchain
- Oracle
- Vaults
---
