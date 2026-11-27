---
api_specs:
- filename: nibgate-xyz-discovery-api-openapi.yml
  format: yaml
  label: Nibgate Discovery API
  slug: nibgate-xyz-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibgate-xyz/openapi/nibgate-xyz-discovery-api-openapi.yml
- filename: nibgate-xyz-jev-api-openapi.yml
  format: yaml
  label: Nibgate JEV API
  slug: nibgate-xyz-jev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibgate-xyz/openapi/nibgate-xyz-jev-api-openapi.yml
- filename: nibgate-xyz-ledger-api-openapi.yml
  format: yaml
  label: Nibgate Ledger API
  slug: nibgate-xyz-ledger-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibgate-xyz/openapi/nibgate-xyz-ledger-api-openapi.yml
- filename: nibgate-xyz-platform-api-openapi.yml
  format: yaml
  label: Nibgate Platform API
  slug: nibgate-xyz-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibgate-xyz/openapi/nibgate-xyz-platform-api-openapi.yml
- filename: nibgate-xyz-reputation-api-openapi.yml
  format: yaml
  label: Nibgate Reputation API
  slug: nibgate-xyz-reputation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibgate-xyz/openapi/nibgate-xyz-reputation-api-openapi.yml
- filename: nibgate-xyz-tips-api-openapi.yml
  format: yaml
  label: Nibgate Tips API
  slug: nibgate-xyz-tips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibgate-xyz/openapi/nibgate-xyz-tips-api-openapi.yml
- filename: nibgate-xyz-unlocks-api-openapi.yml
  format: yaml
  label: Nibgate Unlocks API
  slug: nibgate-xyz-unlocks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nibgate-xyz/openapi/nibgate-xyz-unlocks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: nibgate.xyz
  spf: true
hosts:
- cert_expires: Feb  5 12:25:10 2027 GMT
  host: nibgate.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nibgate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nibgate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Nibgate
provider_slug: nibgate-xyz
slug: nibgate-xyz-domain-security
source_filename: nibgate-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nibgate.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 12:25:10 2027 GMT\n  hsts: false\ndomains:\n- domain: nibgate.xyz\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/nibgate-xyz/security/nibgate-xyz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Paid Content
- USDC
- Arc
- Content Discovery
---
