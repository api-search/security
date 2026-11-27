---
api_specs:
- filename: donethat-ai-openapi-generated.yml
  format: yaml
  label: DoneThat API
  slug: donethat-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/donethat-ai/openapi/_ae-authored/donethat-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: donethat.ai
  spf: true
hosts:
- cert_expires: Jan 31 09:28:19 2027 GMT
  host: donethat.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DoneThat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DoneThat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: DoneThat
provider_slug: donethat-ai
slug: donethat-ai-domain-security
source_filename: donethat-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: donethat.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 09:28:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: donethat.ai\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/donethat-ai/security/donethat-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Time Tracking
- Artificial Intelligence
- Remote Work
- Productivity
---
