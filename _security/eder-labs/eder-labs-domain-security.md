---
api_specs:
- filename: eder-labs-persona-openapi.yml
  format: yaml
  label: Persona API
  slug: persona-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eder-labs/refs/heads/main/openapi/eder-labs-persona-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eder.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: buildpersona.ai
  spf: false
hosts:
- cert_expires: Sep 15 01:00:14 2026 GMT
  host: www.eder.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 12:46:16 2026 GMT
  host: docs.buildpersona.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eder Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eder Labs, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Eder Labs
provider_slug: eder-labs
slug: eder-labs-domain-security
source_filename: eder-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eder.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 01:00:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.buildpersona.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 12:46:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eder.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: buildpersona.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eder-labs/refs/heads/main/security/eder-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Cloud Saas
- AI Agents
- Memory
- Knowledge Graph
- Personalization
- Data Privacy
- Open Source
- Developer Tools
- RAG
---
