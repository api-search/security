---
api_specs:
- filename: asm-co-openapi-generated.yml
  format: yaml
  label: Assembly API
  slug: asm-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asm-co/openapi/_ae-authored/asm-co-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: assembly.com
  spf: true
hosts:
- cert_expires: Dec 31 21:12:23 2026 GMT
  host: assembly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asm Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Assembly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Assembly
provider_slug: asm-co
slug: asm-co-domain-security
source_filename: asm-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: assembly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 21:12:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: assembly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/asm-co/security/asm-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Low-code
- CRM
- AI
- SaaS
---
