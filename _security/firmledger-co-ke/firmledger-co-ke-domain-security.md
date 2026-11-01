---
api_specs:
- filename: firmledger-co-ke-mcp-api-openapi.yml
  format: yaml
  label: FirmLedger MCP API
  slug: firmledger-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmledger-co-ke/openapi/firmledger-co-ke-mcp-api-openapi.yml
- filename: firmledger-co-ke-openapi-generated.yml
  format: yaml
  label: FirmLedger API
  slug: firmledger-co-ke-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmledger-co-ke/openapi/_ae-authored/firmledger-co-ke-openapi-generated.yml
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
  domain: firmledger.co.ke
  spf: true
hosts:
- cert_expires: Dec  3 06:48:15 2026 GMT
  host: firmledger.co.ke
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Firmledger Co Ke Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FirmLedger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: FirmLedger
provider_slug: firmledger-co-ke
slug: firmledger-co-ke-domain-security
source_filename: firmledger-co-ke-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firmledger.co.ke\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 06:48:15 2026 GMT\n  hsts: false\ndomains:\n- domain: firmledger.co.ke\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/firmledger-co-ke/security/firmledger-co-ke-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Directory
- Business-Intelligence
- Kenya
- API
---
