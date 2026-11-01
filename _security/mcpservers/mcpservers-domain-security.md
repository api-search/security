---
api_specs:
- filename: mcpservers-openapi-generated.yml
  format: yaml
  label: mcpservers.org API
  slug: mcpservers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcpservers/openapi/_ae-authored/mcpservers-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mcpservers.org
  spf: true
hosts:
- cert_expires: Jan 16 04:34:15 2027 GMT
  host: mcpservers.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mcpservers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for mcpservers.org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: mcpservers.org
provider_slug: mcpservers
slug: mcpservers-domain-security
source_filename: mcpservers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mcpservers.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 04:34:15 2027 GMT\n  hsts: false\ndomains:\n- domain: mcpservers.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mcpservers/security/mcpservers-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Marketplace
- Integration
- Tools
---
