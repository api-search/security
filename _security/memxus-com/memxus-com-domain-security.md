---
api_specs:
- filename: memxus-com-openapi-generated.yml
  format: yaml
  label: memxus-com API
  slug: memxus-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memxus-com/openapi/_ae-authored/memxus-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: memxus.com
  spf: true
hosts:
- cert_expires: Dec 27 11:52:45 2026 GMT
  host: memxus.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Memxus Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for memxus-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: memxus-com
provider_slug: memxus-com
slug: memxus-com-domain-security
source_filename: memxus-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memxus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 11:52:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: memxus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/memxus-com/security/memxus-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- ContextEngine
- DeveloperTools
- Productivity
- Memory
---
