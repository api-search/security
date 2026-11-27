---
api_specs:
- filename: foxify-pro-openapi-generated.yml
  format: yaml
  label: FOXIFY API
  slug: foxify-pro-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foxify-pro/openapi/_ae-authored/foxify-pro-openapi-generated.yml
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
  dnssec: true
  domain: foxify.pro
  spf: true
hosts:
- cert_expires: Feb  5 10:44:31 2027 GMT
  host: foxify.pro
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FOXIFY Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FOXIFY, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: FOXIFY
provider_slug: foxify-pro
slug: foxify-pro-domain-security
source_filename: foxify-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foxify.pro\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 10:44:31 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: foxify.pro\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/foxify-pro/security/foxify-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Tools
- Agents
- Automation
- Research
- Engineering
---
