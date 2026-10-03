---
api_specs:
- filename: broke2builtai-com-buy-zero-api-openapi.yml
  format: yaml
  label: broke2built Buy Zero API
  slug: broke2builtai-com-buy-zero-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/openapi/broke2builtai-com-buy-zero-api-openapi.yml
- filename: broke2builtai-com-contract-audit-api-openapi.yml
  format: yaml
  label: broke2built Contract Audit API
  slug: broke2builtai-com-contract-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/openapi/broke2builtai-com-contract-audit-api-openapi.yml
- filename: broke2builtai-com-interface-xray-api-openapi.yml
  format: yaml
  label: broke2built Interface Xray API
  slug: broke2builtai-com-interface-xray-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/openapi/broke2builtai-com-interface-xray-api-openapi.yml
- filename: broke2builtai-com-payer-census-api-openapi.yml
  format: yaml
  label: broke2built Payer Census API
  slug: broke2builtai-com-payer-census-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/openapi/broke2builtai-com-payer-census-api-openapi.yml
- filename: broke2builtai-com-payout-oracle-api-openapi.yml
  format: yaml
  label: broke2built Payout Oracle API
  slug: broke2builtai-com-payout-oracle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/openapi/broke2builtai-com-payout-oracle-api-openapi.yml
- filename: broke2builtai-com-resolver-allowlist-api-openapi.yml
  format: yaml
  label: broke2built Resolver Allowlist API
  slug: broke2builtai-com-resolver-allowlist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/openapi/broke2builtai-com-resolver-allowlist-api-openapi.yml
- filename: broke2builtai-com-source-verify-api-openapi.yml
  format: yaml
  label: broke2built Source Verify API
  slug: broke2builtai-com-source-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/openapi/broke2builtai-com-source-verify-api-openapi.yml
- filename: broke2builtai-com-video-api-openapi.yml
  format: yaml
  label: broke2built Video API
  slug: broke2builtai-com-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/openapi/broke2builtai-com-video-api-openapi.yml
- filename: broke2builtai-com-vies-check-api-openapi.yml
  format: yaml
  label: broke2built Vies Check API
  slug: broke2builtai-com-vies-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/openapi/broke2builtai-com-vies-check-api-openapi.yml
- filename: broke2builtai-com-wallet-brief-api-openapi.yml
  format: yaml
  label: broke2built Wallet Brief API
  slug: broke2builtai-com-wallet-brief-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/openapi/broke2builtai-com-wallet-brief-api-openapi.yml
- filename: broke2builtai-com-watch-api-openapi.yml
  format: yaml
  label: broke2built Watch API
  slug: broke2builtai-com-watch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/openapi/broke2builtai-com-watch-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: broke2builtai.com
  spf: true
hosts:
- cert_expires: Nov 25 03:13:59 2026 GMT
  host: broke2builtai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 19:00:40 2026 GMT
  host: api.broke2builtai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 03:51:00 2026 GMT
  host: zero.broke2builtai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Broke2Builtai Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for broke2built, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: broke2built
provider_slug: broke2builtai-com
slug: broke2builtai-com-domain-security
source_filename: broke2builtai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: broke2builtai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 03:13:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.broke2builtai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 19:00:40 2026 GMT\n  hsts: false\n- host: zero.broke2builtai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 03:51:00 2026 GMT\n  hsts: false\ndomains:\n- domain: broke2builtai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/broke2builtai-com/refs/heads/main/security/broke2builtai-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Agents
- Agent Tools
- Data Intelligence
- Domain Intelligence
- Email Verification
- DNS
- SEO
- Web Audits
- Content Extraction
- Blockchain
- EVM
- Base
- Solana
- x402
- Agentic Payments
- A2A
- MCP
- Autonomous Agents
- Agent Networks
- Video Generation
- Monitoring
---
