---
api_specs:
- filename: agentdocs-eu-openapi-generated.yml
  format: yaml
  label: agentdocs-eu API
  slug: agentdocs-eu-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentdocs-eu/openapi/_ae-authored/agentdocs-eu-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentdocs.eu
  spf: true
hosts:
- cert_expires: Dec 22 03:44:36 2026 GMT
  host: agentdocs.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentdocs Eu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for agentdocs-eu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: agentdocs-eu
provider_slug: agentdocs-eu
slug: agentdocs-eu-domain-security
source_filename: agentdocs-eu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentdocs.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 03:44:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agentdocs.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentdocs-eu/security/agentdocs-eu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Collaboration
- Documentation
- AI
- Platform
- OpenSource
- Company
---
