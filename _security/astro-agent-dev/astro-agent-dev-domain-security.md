---
api_specs:
- filename: astro-agent-dev-finance-api-openapi.yml
  format: yaml
  label: astro-agent-dev Finance API
  slug: astro-agent-dev-finance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astro-agent-dev/openapi/astro-agent-dev-finance-api-openapi.yml
- filename: astro-agent-dev-free-api-openapi.yml
  format: yaml
  label: astro-agent-dev Free API
  slug: astro-agent-dev-free-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/astro-agent-dev/openapi/astro-agent-dev-free-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: astro-agent.dev
  spf: false
hosts:
- cert_expires: Jan  1 21:20:17 2027 GMT
  host: astro-agent.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Astro Agent Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for astro-agent-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: astro-agent-dev
provider_slug: astro-agent-dev
slug: astro-agent-dev-domain-security
source_filename: astro-agent-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: astro-agent.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 21:20:17 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: astro-agent.dev\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/astro-agent-dev/security/astro-agent-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AstroFinance
- Astrology
- MarketData
- API
---
