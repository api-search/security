---
api_specs:
- filename: rise-ai-openapi-generated.yml
  format: yaml
  label: Rise.ai API
  slug: rise-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rise-ai/openapi/_ae-authored/rise-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: rise.ai
  spf: true
hosts:
- cert_expires: Dec 30 14:42:03 2026 GMT
  host: rise.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rise Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rise.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Rise.ai
provider_slug: rise-ai
slug: rise-ai-domain-security
source_filename: rise-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rise.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 14:42:03 2026 GMT\n  hsts: null\ndomains:\n- domain: rise.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/rise-ai/security/rise-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
