---
api_specs:
- filename: base167-com-check-api-openapi.yml
  format: yaml
  label: BASE167 Check API
  slug: base167-com-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/base167-com/openapi/base167-com-check-api-openapi.yml
- filename: base167-com-games-api-openapi.yml
  format: yaml
  label: BASE167 Games API
  slug: base167-com-games-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/base167-com/openapi/base167-com-games-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: base167.com
  spf: true
hosts:
- cert_expires: Dec  5 06:52:34 2026 GMT
  host: base167.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BASE167 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BASE167, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BASE167
provider_slug: base167-com
slug: base167-com-domain-security
source_filename: base167-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: base167.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 06:52:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: base167.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/base167-com/security/base167-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Blockchain
- Gaming
- Cryptocurrency
- Tokens
- DegenGames
---
