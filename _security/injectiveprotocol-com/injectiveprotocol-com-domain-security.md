---
api_specs:
- filename: injectiveprotocol-com-injective-api-openapi.yml
  format: yaml
  label: Injective API
  slug: injective-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/injectiveprotocol-com/openapi/injectiveprotocol-com-injective-api-openapi.yml
- filename: injectiveprotocol-com-openapi-generated.yml
  format: yaml
  label: Injective API
  slug: injectiveprotocol-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/injectiveprotocol-com/openapi/_ae-authored/injectiveprotocol-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: injectiveprotocol.com
  spf: true
hosts:
- cert_expires: Jan 22 11:57:38 2027 GMT
  host: injectiveprotocol.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Injectiveprotocol Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Injective, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Injective
provider_slug: injectiveprotocol-com
slug: injectiveprotocol-com-domain-security
source_filename: injectiveprotocol-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: injectiveprotocol.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 11:57:38 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: injectiveprotocol.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/injectiveprotocol-com/security/injectiveprotocol-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Finance
- DeFi
- Infrastructure
- Web3
---
