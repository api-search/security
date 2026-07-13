---
api_specs:
- filename: api-docs.defillama.com
  format: yaml
  label: DefiLlama Hegic Protocol API
  slug: defillama-hegic-protocol-api
  spec_type: OpenAPI
  url: https://api-docs.defillama.com
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hegic.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: defillama.com
  spf: true
hosts:
- cert_expires: Sep  6 02:38:15 2026 GMT
  host: www.hegic.co
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 06:27:35 2026 GMT
  host: defillama.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 20:27:49 2026 GMT
  host: api.llama.fi
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hegic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hegic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hegic
provider_slug: hegic
slug: hegic-domain-security
source_filename: hegic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hegic.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 02:38:15 2026 GMT\n  hsts: false\n- host: defillama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 06:27:35 2026 GMT\n  hsts: false\n- host: api.llama.fi\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 20:27:49 2026 GMT\n  hsts: null\ndomains:\n- domain: hegic.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: defillama.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hegic/refs/heads/main/security/hegic-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- DeFi
- Options Trading
- On-Chain
- Arbitrum
- Ethereum
- Liquidity Pools
- AMM
- Derivatives
- Web3
---
