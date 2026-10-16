---
api_specs:
- filename: zerodha-openapi-generated.yml
  format: yaml
  label: Zerodha API
  slug: zerodha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerodha/refs/heads/main/openapi/_ae-authored/zerodha-openapi-generated.yml
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
- APIs
- Fintech
---
