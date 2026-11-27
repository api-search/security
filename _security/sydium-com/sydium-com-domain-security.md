---
api_specs:
- filename: sydium-com-openapi-generated.yml
  format: yaml
  label: Sydium API
  slug: sydium-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sydium-com/openapi/_ae-authored/sydium-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: sydium.com
  spf: true
hosts:
- cert_expires: Feb  1 17:47:26 2027 GMT
  host: sydium.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sydium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sydium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sydium
provider_slug: sydium-com
slug: sydium-com-domain-security
source_filename: sydium-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sydium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 17:47:26 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sydium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/sydium-com/security/sydium-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Media
- AI
- SaaS
- Marketing
- Automation
---
