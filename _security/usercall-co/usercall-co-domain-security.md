---
api_specs:
- filename: usercall-co-openapi-generated.yml
  format: yaml
  label: Usercall API
  slug: usercall-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usercall-co/openapi/_ae-authored/usercall-co-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-27'
    published: false
  dnssec: false
  domain: usercall.co
  spf: true
hosts:
- cert_expires: Dec 28 00:52:33 2026 GMT
  host: usercall.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Usercall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Usercall, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Usercall
provider_slug: usercall-co
slug: usercall-co-domain-security
source_filename: usercall-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: usercall.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 00:52:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usercall.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-27'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/usercall-co/security/usercall-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Interviews
- Qualitative Analysis
- Research
- Product Management
- Customer Experience
- Market Research
---
