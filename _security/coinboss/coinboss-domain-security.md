---
api_specs:
- filename: coinboss-openapi-generated.yml
  format: yaml
  label: Coin Boss API
  slug: coinboss-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coinboss/openapi/_ae-authored/coinboss-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: coinboss.com
  spf: true
hosts:
- cert_expires: Dec  9 14:07:52 2026 GMT
  host: www.coinboss.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Coin Boss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coin Boss, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Coin Boss
provider_slug: coinboss
slug: coinboss-domain-security
source_filename: coinboss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.coinboss.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 14:07:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: coinboss.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/coinboss/security/coinboss-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cryptocurrency
- Derivatives
- Market Data
- Finance
---
