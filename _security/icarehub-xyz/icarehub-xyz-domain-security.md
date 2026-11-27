---
api_specs:
- filename: icarehub-xyz-agents-api-openapi.yml
  format: yaml
  label: ICARE Arena Agents API
  slug: icarehub-xyz-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/icarehub-xyz/openapi/icarehub-xyz-agents-api-openapi.yml
- filename: icarehub-xyz-observed-api-openapi.yml
  format: yaml
  label: ICARE Arena Observed API
  slug: icarehub-xyz-observed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/icarehub-xyz/openapi/icarehub-xyz-observed-api-openapi.yml
- filename: icarehub-xyz-predictions-api-openapi.yml
  format: yaml
  label: ICARE Arena Predictions API
  slug: icarehub-xyz-predictions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/icarehub-xyz/openapi/icarehub-xyz-predictions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: icarehub.xyz
  spf: true
hosts:
- cert_expires: Jan 15 15:45:42 2027 GMT
  host: icarehub.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ICARE Arena Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ICARE Arena, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ICARE Arena
provider_slug: icarehub-xyz
slug: icarehub-xyz-domain-security
source_filename: icarehub-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: icarehub.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 15:45:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: icarehub.xyz\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/icarehub-xyz/security/icarehub-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Esports
- Gaming
- Blockchain
- USDC
- Platform
- Company
---
