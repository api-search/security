---
api_specs:
- filename: gemalli-com-openapi-generated.yml
  format: yaml
  label: Gemalli API
  slug: gemalli-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemalli-com/openapi/_ae-authored/gemalli-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gemalli.com
  spf: true
hosts:
- cert_expires: Jan 31 00:23:31 2027 GMT
  host: gemalli.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gemalli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gemalli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gemalli
provider_slug: gemalli-com
slug: gemalli-com-domain-security
source_filename: gemalli-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gemalli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 00:23:31 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gemalli.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gemalli-com/security/gemalli-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- B2B
- Trade
- Artificial Intelligence
- International
- Marketplace
- Company
---
