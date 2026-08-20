---
api_specs:
- filename: octav-airdrops-api-openapi.yml
  format: yaml
  label: Octav Airdrops API
  slug: octav-airdrops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-airdrops-api-openapi.yml
- filename: octav-approvals-api-openapi.yml
  format: yaml
  label: Octav Approvals API
  slug: octav-approvals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-approvals-api-openapi.yml
- filename: octav-beacon-validators-api-openapi.yml
  format: yaml
  label: Octav Beacon Validators API
  slug: octav-beacon-validators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-beacon-validators-api-openapi.yml
- filename: octav-chains-api-openapi.yml
  format: yaml
  label: Octav Chains API
  slug: octav-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-chains-api-openapi.yml
- filename: octav-contract-protocol-api-openapi.yml
  format: yaml
  label: Octav Contract Protocol API
  slug: octav-contract-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-contract-protocol-api-openapi.yml
- filename: octav-credits-api-openapi.yml
  format: yaml
  label: Octav Credits API
  slug: octav-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-credits-api-openapi.yml
- filename: octav-nav-api-openapi.yml
  format: yaml
  label: Octav Nav API
  slug: octav-nav-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-nav-api-openapi.yml
- filename: octav-portfolio-api-openapi.yml
  format: yaml
  label: Octav Portfolio API
  slug: octav-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-portfolio-api-openapi.yml
- filename: octav-status-api-openapi.yml
  format: yaml
  label: Octav Status API
  slug: octav-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-status-api-openapi.yml
- filename: octav-sync-api-openapi.yml
  format: yaml
  label: Octav Sync API
  slug: octav-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-sync-api-openapi.yml
- filename: octav-tokens-api-openapi.yml
  format: yaml
  label: Octav Tokens API
  slug: octav-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-tokens-api-openapi.yml
- filename: octav-transactions-api-openapi.yml
  format: yaml
  label: Octav Transactions API
  slug: octav-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-transactions-api-openapi.yml
- filename: octav-virtual-users-api-openapi.yml
  format: yaml
  label: Octav Virtual Users API
  slug: octav-virtual-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-virtual-users-api-openapi.yml
- filename: octav-wallet-api-openapi.yml
  format: yaml
  label: Octav Wallet API
  slug: octav-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octav/refs/heads/main/openapi/octav-wallet-api-openapi.yml
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
- Wallets
---
