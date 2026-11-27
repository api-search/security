---
api_specs:
- filename: lekta-dev-openapi-generated.yml
  format: yaml
  label: Lekta API
  slug: lekta-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lekta-dev/openapi/_ae-authored/lekta-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lekta.dev
  spf: true
hosts:
- cert_expires: Jan  4 14:06:35 2027 GMT
  host: lekta.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lekta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lekta, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lekta
provider_slug: lekta-dev
slug: lekta-dev-domain-security
source_filename: lekta-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lekta.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 14:06:35 2027 GMT\n  hsts: false\ndomains:\n- domain: lekta.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lekta-dev/security/lekta-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Audit
- Readability
- SEO
- Platform
---
