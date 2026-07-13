---
api_specs:
- filename: zinrelo-openapi.yml
  format: yaml
  label: Zinrelo Members API
  slug: zinrelo-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-openapi.yml
- filename: zinrelo-openapi.yml
  format: yaml
  label: Zinrelo Points API
  slug: zinrelo-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-openapi.yml
- filename: zinrelo-openapi.yml
  format: yaml
  label: Zinrelo Transactions API
  slug: zinrelo-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-openapi.yml
- filename: zinrelo-openapi.yml
  format: yaml
  label: Zinrelo Rewards API
  slug: zinrelo-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-openapi.yml
- filename: zinrelo-openapi.yml
  format: yaml
  label: Zinrelo Redemptions API
  slug: zinrelo-redemptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/openapi/zinrelo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: zinrelo.com
  spf: true
hosts:
- cert_expires: Aug 21 00:26:10 2026 GMT
  host: www.zinrelo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 09:46:46 2026 GMT
  host: help.zinrelo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 09:46:46 2026 GMT
  host: api.zinrelo.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zinrelo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zinrelo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zinrelo
provider_slug: zinrelo
slug: zinrelo-domain-security
source_filename: zinrelo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zinrelo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 00:26:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.zinrelo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:46:46 2026 GMT\n  hsts: null\n- host: api.zinrelo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 09:46:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: zinrelo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zinrelo/refs/heads/main/security/zinrelo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Loyalty
- Rewards
- Points
- Customer Retention
- Ecommerce
- SaaS
---
