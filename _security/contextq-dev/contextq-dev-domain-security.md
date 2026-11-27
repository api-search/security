---
api_specs:
- filename: contextq-dev-openapi-generated.yml
  format: yaml
  label: ContextQ API
  slug: contextq-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contextq-dev/openapi/_ae-authored/contextq-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: contextq.dev
  spf: true
hosts:
- cert_expires: Jan  7 10:13:22 2027 GMT
  host: contextq.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ContextQ Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ContextQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ContextQ
provider_slug: contextq-dev
slug: contextq-dev-domain-security
source_filename: contextq-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: contextq.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 10:13:22 2027 GMT\n  hsts: false\ndomains:\n- domain: contextq.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/contextq-dev/security/contextq-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Memory
- Persistent
- Context
- Agents
- Platform
---
