---
api_specs:
- filename: instant-expert-asks-api-openapi.yml
  format: yaml
  label: Instant Expert Asks API
  slug: instant-expert-asks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instant-expert/openapi/instant-expert-asks-api-openapi.yml
- filename: instant-expert-test-mode-api-openapi.yml
  format: yaml
  label: Instant Expert Test mode API
  slug: instant-expert-test-mode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instant-expert/openapi/instant-expert-test-mode-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: instant.expert
  spf: true
hosts:
- cert_expires: Feb  9 23:52:38 2027 GMT
  host: instant.expert
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Instant Expert Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Instant Expert, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Instant Expert
provider_slug: instant-expert
slug: instant-expert-domain-security
source_filename: instant-expert-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: instant.expert\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:52:38 2027 GMT\n  hsts: false\ndomains:\n- domain: instant.expert\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/instant-expert/security/instant-expert-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Outreach
- Sales
- Artificial Intelligence
- MCP
- B2B
---
