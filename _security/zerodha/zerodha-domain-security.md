---
api_specs:
- filename: zerodha-alerts-api-openapi.yml
  format: yaml
  label: Zerodha Alerts API
  slug: zerodha-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerodha/refs/heads/main/openapi/zerodha-alerts-api-openapi.yml
- filename: zerodha-gtt-api-openapi.yml
  format: yaml
  label: Zerodha Gtt API
  slug: zerodha-gtt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerodha/refs/heads/main/openapi/zerodha-gtt-api-openapi.yml
- filename: zerodha-orders-api-openapi.yml
  format: yaml
  label: Zerodha Orders API
  slug: zerodha-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerodha/refs/heads/main/openapi/zerodha-orders-api-openapi.yml
- filename: zerodha-portfolio-api-openapi.yml
  format: yaml
  label: Zerodha Portfolio API
  slug: zerodha-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerodha/refs/heads/main/openapi/zerodha-portfolio-api-openapi.yml
- filename: zerodha-session-api-openapi.yml
  format: yaml
  label: Zerodha Session API
  slug: zerodha-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerodha/refs/heads/main/openapi/zerodha-session-api-openapi.yml
- filename: zerodha-trades-api-openapi.yml
  format: yaml
  label: Zerodha Trades API
  slug: zerodha-trades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerodha/refs/heads/main/openapi/zerodha-trades-api-openapi.yml
- filename: zerodha-user-api-openapi.yml
  format: yaml
  label: Zerodha User API
  slug: zerodha-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerodha/refs/heads/main/openapi/zerodha-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kite.trade
  spf: true
hosts:
- cert_expires: Apr  3 23:59:59 2027 GMT
  host: kite.trade
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zerodha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zerodha, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Zerodha
provider_slug: zerodha
slug: zerodha-domain-security
source_filename: zerodha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kite.trade\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: kite.trade\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerodha/refs/heads/main/security/zerodha-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Finance
- Trading
- Fintech
---
