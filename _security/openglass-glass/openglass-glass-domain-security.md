---
api_specs:
- filename: openglass-glass-agents-api-openapi.yml
  format: yaml
  label: OpenGlass Agents API
  slug: openglass-glass-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-agents-api-openapi.yml
- filename: openglass-glass-attestations-api-openapi.yml
  format: yaml
  label: OpenGlass Attestations API
  slug: openglass-glass-attestations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-attestations-api-openapi.yml
- filename: openglass-glass-auth-api-openapi.yml
  format: yaml
  label: OpenGlass Auth API
  slug: openglass-glass-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-auth-api-openapi.yml
- filename: openglass-glass-claims-api-openapi.yml
  format: yaml
  label: OpenGlass Claims API
  slug: openglass-glass-claims-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-claims-api-openapi.yml
- filename: openglass-glass-invites-api-openapi.yml
  format: yaml
  label: OpenGlass Invites API
  slug: openglass-glass-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-invites-api-openapi.yml
- filename: openglass-glass-meta-api-openapi.yml
  format: yaml
  label: OpenGlass Meta API
  slug: openglass-glass-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-meta-api-openapi.yml
- filename: openglass-glass-owner-api-openapi.yml
  format: yaml
  label: OpenGlass Owner API
  slug: openglass-glass-owner-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-owner-api-openapi.yml
- filename: openglass-glass-records-api-openapi.yml
  format: yaml
  label: OpenGlass Records API
  slug: openglass-glass-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-records-api-openapi.yml
- filename: openglass-glass-sessions-api-openapi.yml
  format: yaml
  label: OpenGlass Sessions API
  slug: openglass-glass-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openglass-glass/openapi/openglass-glass-sessions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openglass.glass
  spf: true
hosts:
- cert_expires: Dec 23 05:40:00 2026 GMT
  host: openglass.glass
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenGlass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenGlass, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenGlass
provider_slug: openglass-glass
slug: openglass-glass-domain-security
source_filename: openglass-glass-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openglass.glass\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 05:40:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openglass.glass\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/openglass-glass/security/openglass-glass-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Data Integrity
- Security
- Agent Platform
- Transparency
---
