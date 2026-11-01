---
api_specs:
- filename: superposition-api-openapi-generated.yml
  format: yaml
  label: Superposition API Reference Authenticate and integrate with the Superposition API. API
  slug: api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superposition/openapi/_ae-authored/superposition-api-openapi-generated.yml
- filename: superposition-core-openapi-generated.yml
  format: yaml
  label: Superposition core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superposition/openapi/_ae-authored/superposition-core-openapi-generated.yml
- filename: superposition-guides-openapi-generated.yml
  format: yaml
  label: Superposition Guides Set up your workspace, create a role, and run your first search. API
  slug: guides-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/superposition/openapi/_ae-authored/superposition-guides-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: superposition.ai
  spf: true
hosts:
- cert_expires: Dec 10 15:01:45 2026 GMT
  host: superposition.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Superposition Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superposition, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Superposition
provider_slug: superposition
slug: superposition-domain-security
source_filename: superposition-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superposition.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 15:01:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: superposition.ai\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/superposition/security/superposition-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Recruiting
- Startup
- Talent
- Hiring
---
