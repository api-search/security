---
api_specs:
- filename: woox-account-api-openapi.yml
  format: yaml
  label: WOO X Account API
  slug: woox-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/openapi/woox-account-api-openapi.yml
- filename: woox-asset-api-openapi.yml
  format: yaml
  label: WOO X Asset API
  slug: woox-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/openapi/woox-asset-api-openapi.yml
- filename: woox-futures-api-openapi.yml
  format: yaml
  label: WOO X Futures API
  slug: woox-futures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/openapi/woox-futures-api-openapi.yml
- filename: woox-isolatedmargin-api-openapi.yml
  format: yaml
  label: WOO X Isolated Margin API
  slug: woox-isolatedmargin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/openapi/woox-isolatedmargin-api-openapi.yml
- filename: woox-public-api-openapi.yml
  format: yaml
  label: WOO X Public API
  slug: woox-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/openapi/woox-public-api-openapi.yml
- filename: woox-spotmargin-api-openapi.yml
  format: yaml
  label: WOO X Spot Margin API
  slug: woox-spotmargin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/openapi/woox-spotmargin-api-openapi.yml
- filename: woox-trade-api-openapi.yml
  format: yaml
  label: WOO X Trade API
  slug: woox-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/openapi/woox-trade-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: woox.io
  spf: true
hosts:
- cert_expires: Dec  9 14:38:08 2026 GMT
  host: woox.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Woox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WOO X, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: WOO X
provider_slug: woox
slug: woox-domain-security
source_filename: woox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: woox.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 14:38:08 2026 GMT\n  hsts: false\ndomains:\n- domain: woox.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/woox/refs/heads/main/security/woox-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Exchanges
- Trading
- Derivatives
---
