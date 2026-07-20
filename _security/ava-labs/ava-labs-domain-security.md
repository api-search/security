---
api_specs:
- filename: ava-labs-data-api-openapi.yml
  format: yaml
  label: AvaCloud Data API
  slug: avacloud-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-labs/refs/heads/main/openapi/ava-labs-data-api-openapi.yml
- filename: ava-labs-metrics-api-openapi.yml
  format: yaml
  label: AvaCloud Metrics API
  slug: avacloud-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-labs/refs/heads/main/openapi/ava-labs-metrics-api-openapi.yml
- filename: ava-labs-platform-api-openapi.yml
  format: yaml
  label: Avalanche Platform Chain API
  slug: avalanche-platform-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ava-labs/refs/heads/main/openapi/ava-labs-platform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: avalabs.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: avax.network
  spf: true
hosts:
- cert_expires: Sep 29 16:26:09 2026 GMT
  host: avalabs.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 22:05:14 2026 GMT
  host: glacier-api.avax.network
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 22:05:14 2026 GMT
  host: metrics.avax.network
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ava Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ava Labs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ava Labs
provider_slug: ava-labs
slug: ava-labs-domain-security
source_filename: ava-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avalabs.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 16:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: glacier-api.avax.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 22:05:14 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: metrics.avax.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 22:05:14 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: avalabs.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: avax.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ava-labs/refs/heads/main/security/ava-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Crypto
- Blockchain
- Avalanche
- Web3
- Data API
- Developer Platform
- Infrastructure
---
