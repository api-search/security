---
api_specs:
- filename: joxo-ai-openapi-generated.yml
  format: yaml
  label: Joxo API
  slug: joxo-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joxo-ai/openapi/_ae-authored/joxo-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: joxo.ai
  spf: true
hosts:
- cert_expires: Feb  5 12:14:37 2027 GMT
  host: joxo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Joxo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Joxo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Joxo
provider_slug: joxo-ai
slug: joxo-ai-domain-security
source_filename: joxo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joxo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 12:14:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: joxo.ai\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/joxo-ai/security/joxo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Agents
- Workspace
- Enterprise
- Security
---
