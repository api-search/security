---
api_specs:
- filename: connext-batched-intents-api-openapi.yml
  format: yaml
  label: Everclear Batched Intents API
  slug: connext-batched-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-batched-intents-api-openapi.yml
- filename: connext-configs-api-openapi.yml
  format: yaml
  label: Everclear Configs API
  slug: connext-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-configs-api-openapi.yml
- filename: connext-history-api-openapi.yml
  format: yaml
  label: Everclear History API
  slug: connext-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-history-api-openapi.yml
- filename: connext-intents-api-openapi.yml
  format: yaml
  label: Everclear Intents API
  slug: connext-intents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-intents-api-openapi.yml
- filename: connext-invoices-api-openapi.yml
  format: yaml
  label: Everclear Invoices API
  slug: connext-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-invoices-api-openapi.yml
- filename: connext-routes-api-openapi.yml
  format: yaml
  label: Everclear Routes API
  slug: connext-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-routes-api-openapi.yml
- filename: connext-solana-api-openapi.yml
  format: yaml
  label: Everclear Solana API
  slug: connext-solana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-solana-api-openapi.yml
- filename: connext-tron-api-openapi.yml
  format: yaml
  label: Everclear Tron API
  slug: connext-tron-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/openapi/connext-tron-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: connext.network
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: everclear.org
  spf: true
hosts:
- cert_expires: Nov  7 15:12:44 2026 GMT
  host: www.connext.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 01:58:58 2026 GMT
  host: docs.everclear.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 10:09:46 2026 GMT
  host: api.everclear.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Connext Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Everclear, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Everclear
provider_slug: connext
slug: connext-domain-security
source_filename: connext-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.connext.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 15:12:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.everclear.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 01:58:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.everclear.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 10:09:46 2026 GMT\n  hsts: null\ndomains:\n- domain: connext.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: everclear.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connext/refs/heads/main/security/connext-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Cryptocurrency
- Web3
- Interoperability
- Cross-Chain
- Bridging
- Settlement
- Liquidity
- Intents
- DeFi
- Chain Abstraction
- Defunct
---
