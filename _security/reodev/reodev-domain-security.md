---
api_specs:
- filename: reodev-openapi-generated.yml
  format: yaml
  label: Reo.dev API
  slug: reodev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/reodev/openapi/_ae-authored/reodev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: reo.dev
  spf: true
hosts:
- cert_expires: Jan  7 22:46:31 2027 GMT
  host: www.reo.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Reodev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reo.dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Reo.dev
provider_slug: reodev
slug: reodev-domain-security
source_filename: reodev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 22:46:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reo.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/reodev/security/reodev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- low-code
- API-platform
- integration
- developer-tools
- startup
---
