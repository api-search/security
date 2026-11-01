---
api_specs:
- filename: supermemory-openapi.json
  format: json
  label: Supermemory API
  slug: supermemory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/supermemory/openapi/supermemory-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: supermemory.ai
  spf: true
hosts:
- cert_expires: Jan 14 00:07:33 2027 GMT
  host: supermemory.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Supermemory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Supermemory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Supermemory
provider_slug: supermemory
slug: supermemory-domain-security
source_filename: supermemory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: supermemory.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 00:07:33 2027 GMT\n  hsts: false\ndomains:\n- domain: supermemory.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/supermemory/security/supermemory-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Memory
- Agents
- Platform
---
