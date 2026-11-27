---
api_specs:
- filename: teste-no-openapi-generated.yml
  format: yaml
  label: Teste.no API
  slug: teste-no-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/teste-no/openapi/_ae-authored/teste-no-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: teste.no
  spf: false
hosts:
- cert_expires: Dec 27 01:34:32 2026 GMT
  host: teste.no
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Teste.no Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teste.no, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Teste.no
provider_slug: teste-no
slug: teste-no-domain-security
source_filename: teste-no-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teste.no\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 01:34:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: teste.no\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/teste-no/security/teste-no-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Monitoring
- Testing
- Security
- Performance
- SEO
- Accessibility
- E‑commerce
- API
---
