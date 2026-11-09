---
api_specs:
- filename: firstresponder-guide-openapi-generated.yml
  format: yaml
  label: First Responder Guide API
  slug: firstresponder-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firstresponder-guide/openapi/_ae-authored/firstresponder-guide-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: firstresponder.guide
  spf: false
hosts:
- cert_expires: Dec 31 18:24:25 2026 GMT
  host: firstresponder.guide
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Firstresponder Guide Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First Responder Guide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: First Responder Guide
provider_slug: firstresponder-guide
slug: firstresponder-guide-domain-security
source_filename: firstresponder-guide-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: firstresponder.guide\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 18:24:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: firstresponder.guide\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/firstresponder-guide/security/firstresponder-guide-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Public Safety
- Guides
- Education
- Resilience
- Community
---
