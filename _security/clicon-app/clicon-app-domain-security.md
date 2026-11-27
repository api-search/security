---
api_specs:
- filename: clicon-app-openapi-generated.yml
  format: yaml
  label: Clicon Lotus Bot Tracking API
  slug: clicon-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clicon-app/openapi/_ae-authored/clicon-app-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clicon.app
  spf: true
hosts:
- cert_expires: Dec 25 12:24:25 2026 GMT
  host: clicon.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Clicon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clicon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clicon
provider_slug: clicon-app
slug: clicon-app-domain-security
source_filename: clicon-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clicon.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 12:24:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: clicon.app\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/clicon-app/security/clicon-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Generative Engine Optimization
- MCP
- AI Crawlers
- Analytics
- BusinessTools
- SEO
---
