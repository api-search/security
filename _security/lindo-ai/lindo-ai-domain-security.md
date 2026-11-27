---
api_specs:
- filename: lindo-ai-api-openapi.json
  format: json
  label: Lindo Unified API API
  slug: lindo-unified-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lindo-ai/openapi/_original/lindo-ai-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lindo.ai
  spf: true
hosts:
- cert_expires: Feb  4 03:38:38 2027 GMT
  host: lindo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: lindo.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lindo.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: lindo.ai
provider_slug: lindo-ai
slug: lindo-ai-domain-security
source_filename: lindo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lindo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 03:38:38 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lindo.ai\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lindo-ai/security/lindo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Website Builder
- White Label
- Automation
- Software-as-a-Service
---
