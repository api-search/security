---
api_specs:
- filename: contio-ai-openapi-generated.yml
  format: yaml
  label: Contio API
  slug: contio-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contio-ai/openapi/_ae-authored/contio-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: contio.ai
  spf: true
hosts:
- cert_expires: Jan 27 11:13:10 2027 GMT
  host: contio.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Contio Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Contio
provider_slug: contio-ai
slug: contio-ai-domain-security
source_filename: contio-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contio.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 11:13:10 2027 GMT\n  hsts: false\ndomains:\n- domain: contio.ai\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/contio-ai/security/contio-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Productivity
- Meetings
- Software-as-a-Service
- Collaboration
---
