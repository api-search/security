---
api_specs:
- filename: brapi-openapi.yml
  format: yaml
  label: brapi Quotes API
  slug: quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brapi/refs/heads/main/openapi/brapi-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: brapi.dev
  spf: true
hosts:
- cert_expires: Sep 15 05:17:04 2026 GMT
  host: brapi.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for brapi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: brapi
provider_slug: brapi
slug: brapi-domain-security
source_filename: brapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brapi.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 05:17:04 2026 GMT\n  hsts: false\ndomains:\n- domain: brapi.dev\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brapi/refs/heads/main/security/brapi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Finance
- Brazilian Financial Data
- Stock Market
- Investments
- Economic Indicators
- Cryptocurrency
---
