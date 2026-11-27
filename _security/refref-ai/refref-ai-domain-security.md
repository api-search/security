---
api_specs:
- filename: refref-ai-openapi-generated.yml
  format: yaml
  label: RefRef API
  slug: refref-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/refref-ai/openapi/_ae-authored/refref-ai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: refref.ai
  spf: true
hosts:
- cert_expires: Feb  1 10:21:50 2027 GMT
  host: refref.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: RefRef Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RefRef, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RefRef
provider_slug: refref-ai
slug: refref-ai-domain-security
source_filename: refref-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: refref.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 10:21:50 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: refref.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/refref-ai/security/refref-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Referral
- Affiliate
- Loyalty
- OpenSource
- SaaS
---
