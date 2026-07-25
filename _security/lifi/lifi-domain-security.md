---
api_specs:
- filename: lifi-advanced-api-openapi.yml
  format: yaml
  label: LI.FI advanced API
  slug: lifi-advanced-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-advanced-api-openapi.yml
- filename: lifi-analytics-api-openapi.yml
  format: yaml
  label: LI.FI Analytics API
  slug: lifi-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-analytics-api-openapi.yml
- filename: lifi-calldata-api-openapi.yml
  format: yaml
  label: LI.FI Calldata API
  slug: lifi-calldata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-calldata-api-openapi.yml
- filename: lifi-chains-api-openapi.yml
  format: yaml
  label: LI.FI Chains API
  slug: lifi-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-chains-api-openapi.yml
- filename: lifi-connections-api-openapi.yml
  format: yaml
  label: LI.FI Connections API
  slug: lifi-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-connections-api-openapi.yml
- filename: lifi-earn-chains-api-openapi.yml
  format: yaml
  label: LI.FI Earn Chains API
  slug: lifi-earn-chains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-earn-chains-api-openapi.yml
- filename: lifi-earn-portfolio-api-openapi.yml
  format: yaml
  label: LI.FI Earn Portfolio API
  slug: lifi-earn-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-earn-portfolio-api-openapi.yml
- filename: lifi-earn-protocols-api-openapi.yml
  format: yaml
  label: LI.FI Earn Protocols API
  slug: lifi-earn-protocols-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-earn-protocols-api-openapi.yml
- filename: lifi-earn-vaults-api-openapi.yml
  format: yaml
  label: LI.FI Earn Vaults API
  slug: lifi-earn-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-earn-vaults-api-openapi.yml
- filename: lifi-gas-api-openapi.yml
  format: yaml
  label: LI.FI Gas API
  slug: lifi-gas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-gas-api-openapi.yml
- filename: lifi-integrators-api-openapi.yml
  format: yaml
  label: LI.FI Integrators API
  slug: lifi-integrators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-integrators-api-openapi.yml
- filename: lifi-quote-api-openapi.yml
  format: yaml
  label: LI.FI Quote API
  slug: lifi-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-quote-api-openapi.yml
- filename: lifi-relayer-api-openapi.yml
  format: yaml
  label: LI.FI Relayer API
  slug: lifi-relayer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-relayer-api-openapi.yml
- filename: lifi-status-api-openapi.yml
  format: yaml
  label: LI.FI Status API
  slug: lifi-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-status-api-openapi.yml
- filename: lifi-token-api-openapi.yml
  format: yaml
  label: LI.FI Token API
  slug: lifi-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-token-api-openapi.yml
- filename: lifi-tokens-api-openapi.yml
  format: yaml
  label: LI.FI Tokens API
  slug: lifi-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-tokens-api-openapi.yml
- filename: lifi-tools-api-openapi.yml
  format: yaml
  label: LI.FI Tools API
  slug: lifi-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/openapi/lifi-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: li.fi
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: li.quest
  spf: false
hosts:
- cert_expires: Oct 16 05:07:49 2026 GMT
  host: li.fi
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 17:26:58 2026 GMT
  host: earn.li.fi
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 15:16:44 2026 GMT
  host: li.quest
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lifi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LI.FI, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: LI.FI
provider_slug: lifi
slug: lifi-domain-security
source_filename: lifi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: li.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 05:07:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: earn.li.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 17:26:58 2026 GMT\n  hsts: null\n- host: li.quest\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 15:16:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: li.fi\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: li.quest\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifi/refs/heads/main/security/lifi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto Web3
- Blockchain
- Cross-Chain
- Bridges
- DEX Aggregation
- DeFi
- Payments
- Liquidity
- Yield
- Intents
- Agents
---
