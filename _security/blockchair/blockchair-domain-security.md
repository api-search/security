---
api_specs:
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Address Dashboards API
  slug: address-dashboards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Transaction Dashboards API
  slug: transaction-dashboards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Block Dashboards API
  slug: block-dashboards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Raw Data API
  slug: raw-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Stats API
  slug: stats
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Outputs Database API
  slug: outputs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
- filename: blockchair-openapi.yml
  format: yaml
  label: Blockchair Broadcast API
  slug: broadcast
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/openapi/blockchair-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:admin@blockchair.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: blockchair.com
  spf: true
hosts:
- cert_expires: Sep 18 14:33:07 2026 GMT
  host: blockchair.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 06:00:23 2026 GMT
  host: api.blockchair.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Blockchair Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blockchair, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Blockchair
provider_slug: blockchair
slug: blockchair-domain-security
source_filename: blockchair-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blockchair.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 14:33:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.blockchair.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 13 06:00:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: blockchair.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:admin@blockchair.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockchair/refs/heads/main/security/blockchair-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Cryptocurrency
- Explorer
- Bitcoin
- Ethereum
- On-Chain Data
---
