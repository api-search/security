---
api_specs:
- filename: kadena-block-api-openapi.yml
  format: yaml
  label: Kadena block API
  slug: kadena-block-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-block-api-openapi.yml
- filename: kadena-blockhash-api-openapi.yml
  format: yaml
  label: Kadena blockhash API
  slug: kadena-blockhash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-blockhash-api-openapi.yml
- filename: kadena-config-api-openapi.yml
  format: yaml
  label: Kadena config API
  slug: kadena-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-config-api-openapi.yml
- filename: kadena-cut-api-openapi.yml
  format: yaml
  label: Kadena cut API
  slug: kadena-cut-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-cut-api-openapi.yml
- filename: kadena-endpoint-listen-api-openapi.yml
  format: yaml
  label: Kadena endpoint-listen API
  slug: kadena-endpoint-listen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-listen-api-openapi.yml
- filename: kadena-endpoint-local-api-openapi.yml
  format: yaml
  label: Kadena endpoint-local API
  slug: kadena-endpoint-local-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-local-api-openapi.yml
- filename: kadena-endpoint-poll-api-openapi.yml
  format: yaml
  label: Kadena endpoint-poll API
  slug: kadena-endpoint-poll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-poll-api-openapi.yml
- filename: kadena-endpoint-private-api-openapi.yml
  format: yaml
  label: Kadena endpoint-private API
  slug: kadena-endpoint-private-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-private-api-openapi.yml
- filename: kadena-endpoint-send-api-openapi.yml
  format: yaml
  label: Kadena endpoint-send API
  slug: kadena-endpoint-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-send-api-openapi.yml
- filename: kadena-endpoint-spv-api-openapi.yml
  format: yaml
  label: Kadena endpoint-spv API
  slug: kadena-endpoint-spv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-endpoint-spv-api-openapi.yml
- filename: kadena-header-api-openapi.yml
  format: yaml
  label: Kadena header API
  slug: kadena-header-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-header-api-openapi.yml
- filename: kadena-mempool-api-openapi.yml
  format: yaml
  label: Kadena mempool API
  slug: kadena-mempool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-mempool-api-openapi.yml
- filename: kadena-mining-api-openapi.yml
  format: yaml
  label: Kadena mining API
  slug: kadena-mining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-mining-api-openapi.yml
- filename: kadena-misc-api-openapi.yml
  format: yaml
  label: Kadena misc API
  slug: kadena-misc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-misc-api-openapi.yml
- filename: kadena-payload-api-openapi.yml
  format: yaml
  label: Kadena payload API
  slug: kadena-payload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-payload-api-openapi.yml
- filename: kadena-peer-api-openapi.yml
  format: yaml
  label: Kadena peer API
  slug: kadena-peer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/openapi/kadena-peer-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kadena.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: chainweb.com
  spf: false
hosts:
- cert_expires: Aug 21 16:00:08 2026 GMT
  host: kadena.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 03:02:25 2026 GMT
  host: docs.kadena.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.chainweb.com
  https: false
kind: domain-security
layout: security
method: probed
name: Kadena Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kadena, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kadena
provider_slug: kadena
slug: kadena-domain-security
source_filename: kadena-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kadena.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 16:00:08 2026 GMT\n  hsts: null\n- host: docs.kadena.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 03:02:25 2026 GMT\n  hsts: null\n- host: api.chainweb.com\n  https: false\ndomains:\n- domain: kadena.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: chainweb.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kadena/refs/heads/main/security/kadena-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto Web3
- Blockchain
- Smart Contracts
- Proof of Work
- Layer 1
- Web3
- Cryptocurrency
- Developer Tools
- Decentralized
---
