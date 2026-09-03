---
api_specs:
- filename: ankr-evm-api-openapi.yml
  format: yaml
  label: ankr EVM API
  slug: ankr-evm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-evm-api-openapi.yml
- filename: ankr-metrics-api-openapi.yml
  format: yaml
  label: ankr Metrics API
  slug: ankr-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-metrics-api-openapi.yml
- filename: ankr-nft-api-openapi.yml
  format: yaml
  label: ankr NFT API
  slug: ankr-nft-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-nft-api-openapi.yml
- filename: ankr-query-api-openapi.yml
  format: yaml
  label: ankr Query API
  slug: ankr-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-query-api-openapi.yml
- filename: ankr-ratio-api-openapi.yml
  format: yaml
  label: ankr Ratio API
  slug: ankr-ratio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-ratio-api-openapi.yml
- filename: ankr-tasks-api-openapi.yml
  format: yaml
  label: ankr Tasks API
  slug: ankr-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-tasks-api-openapi.yml
- filename: ankr-token-api-openapi.yml
  format: yaml
  label: ankr Token API
  slug: ankr-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-token-api-openapi.yml
- filename: ankr-validators-api-openapi.yml
  format: yaml
  label: ankr Validators API
  slug: ankr-validators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/openapi/ankr-validators-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ankr.com
  spf: true
hosts:
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: www.ankr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 17:50:31 2026 GMT
  host: rpc.ankr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 07:25:16 2026 GMT
  host: api.staking.ankr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ankr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ankr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ankr
provider_slug: ankr
slug: ankr-domain-security
source_filename: ankr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ankr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rpc.ankr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 17:50:31 2026 GMT\n  hsts: null\n- host: api.staking.ankr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 07:25:16 2026 GMT\n  hsts: null\ndomains:\n- domain: ankr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/security/ankr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
