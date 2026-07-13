---
api_specs:
- filename: grapes-finance-openapi.yml
  format: yaml
  label: Grapes Finance Core API (Master Vintner)
  slug: grapes-finance-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grapes-finance/refs/heads/main/openapi/grapes-finance-openapi.yml
- filename: grapes-finance-openapi.yml
  format: yaml
  label: Grapes Finance Organizations API (Vineyard Manager)
  slug: grapes-finance-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grapes-finance/refs/heads/main/openapi/grapes-finance-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: grapesfinance.com
  spf: true
hosts:
- cert_expires: Sep 21 17:46:51 2026 GMT
  host: docs.grapesfinance.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- host: api.demo.grapesfinance.com
  https: false
kind: domain-security
layout: security
method: probed
name: Grapes Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grapes Finance, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Grapes Finance
provider_slug: grapes-finance
slug: grapes-finance-domain-security
source_filename: grapes-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.grapesfinance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 17:46:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: api.demo.grapesfinance.com\n  https: false\ndomains:\n- domain: grapesfinance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grapes-finance/refs/heads/main/security/grapes-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Stablecoin
- Onramp
- Offramp
- Fiat
- Payments
- Cryptocurrency
- Embedded Finance
---
