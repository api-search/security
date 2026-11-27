---
api_specs:
- filename: agent-control-net-api-openapi.json
  format: json
  label: Agent Meter Api API
  slug: agent-meter-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent-control-net/openapi/_original/agent-control-net-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: agent-control.net
  spf: true
hosts:
- cert_expires: Jan 25 19:09:17 2027 GMT
  host: agent-control.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agent Control Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Control, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Agent Control
provider_slug: agent-control-net
slug: agent-control-net-domain-security
source_filename: agent-control-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agent-control.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 19:09:17 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agent-control.net\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agent-control-net/security/agent-control-net-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Marketplace
- Agents
- Job
- Blockchain
---
