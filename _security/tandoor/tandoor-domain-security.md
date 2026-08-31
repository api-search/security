---
api_specs:
- filename: tandoor-api-api-openapi.yml
  format: yaml
  label: Tandoor Recipes API
  slug: tandoor-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tandoor/refs/heads/main/openapi/tandoor-api-api-openapi.yml
- filename: tandoor-api-token-auth-api-openapi.yml
  format: yaml
  label: Tandoor Recipes API Token Auth API
  slug: tandoor-api-token-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tandoor/refs/heads/main/openapi/tandoor-api-token-auth-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tandoor.dev
  spf: true
hosts:
- cert_expires: Oct 22 05:56:11 2026 GMT
  host: tandoor.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 13:45:18 2026 GMT
  host: docs.tandoor.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 05:55:56 2026 GMT
  host: app.tandoor.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tandoor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tandoor Recipes, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tandoor Recipes
provider_slug: tandoor
slug: tandoor-domain-security
source_filename: tandoor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tandoor.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 05:56:11 2026 GMT\n  hsts: false\n- host: docs.tandoor.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 13:45:18 2026 GMT\n  hsts: false\n- host: app.tandoor.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 05:55:56 2026 GMT\n  hsts: false\ndomains:\n- domain: tandoor.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tandoor/refs/heads/main/security/tandoor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- recipes
- meal-planning
- food
- nutrition
- shopping-lists
- Open-Source
- self-hosted
- home-automation
- django
- Open Data
---
