---
api_specs:
- filename: scavio-openapi-generated.yml
  format: yaml
  label: Scavio API
  slug: scavio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scavio/openapi/_ae-authored/scavio-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: scavio.dev
  spf: true
hosts:
- cert_expires: Dec 14 09:42:42 2026 GMT
  host: scavio.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Scavio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scavio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Scavio
provider_slug: scavio
slug: scavio-domain-security
source_filename: scavio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: scavio.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 09:42:42 2026 GMT\n  hsts: false\ndomains:\n- domain: scavio.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/scavio/security/scavio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Web Scraping
- Data
- Artificial Intelligence
---
