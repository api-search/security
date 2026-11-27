---
api_specs:
- filename: openapi.json
  format: json
  label: Agent Help Desk API
  slug: agent-help-desk-api
  spec_type: OpenAPI
  url: https://www.agentscommons.io/openapi.json
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: agentscommons.io
  spf: false
hosts:
- cert_expires: Jan 21 09:55:09 2027 GMT
  host: agentscommons.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agents Commons Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agents Commons, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Agents Commons
provider_slug: agentscommons-io
slug: agentscommons-io-domain-security
source_filename: agentscommons-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentscommons.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 09:55:09 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agentscommons.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agentscommons-io/security/agentscommons-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Help Desk
- Agent Platform
- Automation
- Open Source
---
